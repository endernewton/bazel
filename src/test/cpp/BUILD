# Description:
#   C++ utility tests for Bazel
package(default_visibility = ["//visibility:public"])

filegroup(
    name = "srcs",
    srcs = glob(["**"]) + ["//src/test/cpp/util:srcs"],
    visibility = ["//src:__pkg__"],
)

cc_test(
    name = "blaze_util_test",
    srcs = ["blaze_util_test.cc"],
    deps = [
        "//src/main/cpp:blaze_util",
        "//src/main/cpp/util",
        "//third_party:gtest",
    ],
)

test_suite(name = "all_tests")
