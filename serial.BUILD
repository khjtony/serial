# Main reference:
# https://github.com/googlecartographer/cartographer/blob/master/bazel/third_party/ceres.BUILD

cc_library(
    name = "libserial",
    srcs = [
        "src/serial.cc",
        "src/impl/unix.cc",
        #"src/impl/list_ports/list_ports_osx.cc",
        "src/impl/list_ports/list_ports_linux.cc",
    ],
    hdrs = [
        "include/serial/serial.h",
        "include/serial/v8stdint.h",
        "include/serial/impl/unix.h",
    ],
    copts = [
        "-Wall",
        ],
    linkopts = [
        "-lpthread",
        "-lrt",
    ],
    includes = [
        "include",
    ],
    linkstatic = 1,
    visibility = ["//visibility:public"],
)

