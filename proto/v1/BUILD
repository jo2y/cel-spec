package(
    # default_compatible_with = ["//buildenv/target:appengine"],
    default_visibility = ["//visibility:public"],
)

licenses(["notice"])  # Apache 2.0

exports_files(["LICENSE"])

proto_library(
    name = "value_protos",
    srcs = [
        "value.proto",
    ],
    # cc_api_version = 2,
    # java_api_version = 2,
    # js_api_version = 2,
    deps = [
        "@com_google_protobuf//:any_proto",
        "@com_google_protobuf//:duration_proto",
        "@com_google_protobuf//:empty_proto",
        "@com_google_protobuf//:struct_proto",
        "@com_google_protobuf//:timestamp_proto",
    ],
)

java_proto_library(
    name = "value_java_proto",
    deps = [":value_protos"],
)

java_lite_proto_library(
    name = "value_java_proto_lite",
    deps = [":value_protos"],
)

proto_library(
    name = "eval_protos",
    srcs = [
        "eval.proto",
    ],
    # cc_api_version = 2,
    # java_api_version = 2,
    # js_api_version = 2,
    deps = [
        ":value_protos",
        "@com_google_googleapis//:rpc_status",
    ],
)

java_proto_library(
    name = "eval_java_proto",
    deps = [":eval_protos"],
)

java_lite_proto_library(
    name = "eval_java_proto_lite",
    deps = [":eval_protos"],
)

proto_library(
    name = "syntax_protos",
    srcs = [
        "syntax.proto",
    ],
    # cc_api_version = 2,
    # java_api_version = 2,
    # js_api_version = 2,
    deps = [
        "@com_google_protobuf//:any_proto",
        "@com_google_protobuf//:duration_proto",
        "@com_google_protobuf//:empty_proto",
        "@com_google_protobuf//:struct_proto",
        "@com_google_protobuf//:timestamp_proto",
    ],
)

java_proto_library(
    name = "syntax_java_proto",
    deps = [":syntax_protos"],
)

java_lite_proto_library(
    name = "syntax_java_proto_lite",
    deps = [":syntax_protos"],
)
