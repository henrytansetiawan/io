licenses(["notice"])  # Apache 2.0

package(default_visibility = ["//visibility:public"])

load(
    "//tensorflow_io:tensorflow_io.bzl",
    "tf_io_copts",
)

cc_library(
    name = "lmdb_ops",
    srcs = [
        "kernels/lmdb_input.cc",
        "ops/lmdb_ops.cc",
    ],
    copts = tf_io_copts(),
    linkstatic = True,
    deps = [
        "//tensorflow_io/core:dataset_ops",
        "@lmdb",
    ],
)
