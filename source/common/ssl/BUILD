licenses(["notice"])  # Apache 2

load(
    "//bazel:envoy_build_system.bzl",
    "envoy_cc_library",
    "envoy_package",
)

envoy_package()

envoy_cc_library(
    name = "tls_certificate_config_impl_lib",
    srcs = ["tls_certificate_config_impl.cc"],
    hdrs = ["tls_certificate_config_impl.h"],
    deps = [
        "//include/envoy/server:transport_socket_config_interface",
        "//include/envoy/ssl:tls_certificate_config_interface",
        "//include/envoy/ssl/private_key:private_key_interface",
        "//source/common/common:empty_string",
        "//source/common/config:datasource_lib",
        "@envoy_api//envoy/api/v2/auth:pkg_cc_proto",
    ],
)

envoy_cc_library(
    name = "certificate_validation_context_config_impl_lib",
    srcs = ["certificate_validation_context_config_impl.cc"],
    hdrs = ["certificate_validation_context_config_impl.h"],
    deps = [
        "//include/envoy/api:api_interface",
        "//include/envoy/ssl:certificate_validation_context_config_interface",
        "//source/common/common:empty_string",
        "//source/common/config:datasource_lib",
        "@envoy_api//envoy/api/v2/auth:pkg_cc_proto",
    ],
)
