licenses(["notice"])  # Apache 2

load(
    "//bazel:envoy_build_system.bzl",
    "envoy_cc_library",
    "envoy_package",
)

envoy_package()

envoy_cc_library(
    name = "utility_lib",
    srcs = [
        "crypto_impl.cc",
        "utility.cc",
    ],
    hdrs = [
        "crypto_impl.h",
    ],
    external_deps = [
        "ssl",
    ],
    deps = [
        "//include/envoy/buffer:buffer_interface",
        "//source/common/common:assert_lib",
        "//source/common/common:stack_array",
        "//source/common/crypto:utility_lib",
    ],
)
