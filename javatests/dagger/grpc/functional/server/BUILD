# Functional tests for Dagger-gRPC

load("@rules_java//java:defs.bzl", "java_proto_library")
load("//:build_defs.bzl", "DOCLINT_HTML_AND_SYNTAX", "DOCLINT_REFERENCES")
load("//:test_defs.bzl", "GenJavaTests")

package(default_visibility = ["//:src"])

# TODO(dpb): enable tests once java_grpc_library is ready in bazel:
# https://github.com/grpc/grpc-java/issues/2756

java_proto_library(
    name = "coffee_service_java_proto",
    deps = [":protos"],
)

proto_library(
    name = "protos",
    srcs = glob(["*.proto"]),
)
