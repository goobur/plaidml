load(
    "//bzl:plaidml.bzl",
    "plaidml_cc_library",
    "plaidml_cc_test",
)

plaidml_cc_test(
    name = "test",
    srcs = [
        "math_test.cc",
        "test.cc",
    ],
    deps = [
        ":math",
    ],
)

plaidml_cc_library(
    name = "math",
    srcs = [
        "basis.cc",
        "bignum.cc",
        "matrix.cc",
        "polynomial.cc",
    ],
    hdrs = [
        "basis.h",
        "bignum.h",
        "matrix.h",
        "polynomial.h",
        "util.h",
    ],
    visibility = ["//visibility:public"],
    deps = [
        "//base/util",
        "@boost",
    ],
)
