package(default_visibility = ["//visibility:public"])

load("//:compiler_options.bzl", "hardball_compiler_flags")

cc_library(
    name = "zipper",
    srcs = glob(
        [
            "**/*.cpp",
            "**/*.c",
        ],
    ),
    hdrs = glob([
        "**/*.h",
    ]),
    copts = hardball_compiler_flags + [
        "-Wno-duplicated-branches",
    ],
    deps = [
        "@zzlib//:zlib",
    ],
)
