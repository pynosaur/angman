load("@rules_python//python:defs.bzl", "py_binary")

py_binary(
    name = "angman",
    srcs = glob(["app/**/*.py"]),
    main = "app/main.py",
    visibility = ["//visibility:public"],
)

genrule(
    name = "angman_binary",
    srcs = glob(["app/**/*.py"]) + [".program", "doc/angman.yaml"],
    outs = ["angman_bin"],
    cmd = """
        python -m nuitka \
            --onefile \
            --output-dir=$(@D) \
            --output-filename=angman \
            app/main.py
        cp $(@D)/angman $@
    """,
    visibility = ["//visibility:public"],
)
