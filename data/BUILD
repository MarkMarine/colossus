java_library(
    name = "data_java_lib",
    srcs = ["DataHandler.java"],
    visibility = ["//visibility:public"],
    deps = [
        "//external:grpc-core",
        "//external:grpc-netty",
        "//external:grpc-stub",
        "//proto/data:data_java_grpc",
        "//proto/data:data_java_proto",
        "@io_prometheus_simpleclient//jar",
        "@io_prometheus_simpleclient_httpserver//jar",
        "@me_dinowernli_java_grpc_prometheus//jar",
    ],
)

java_binary(
    name = "data_java_bin",
    main_class = "colossus.DataHandler",
    visibility = ["//visibility:public"],
    runtime_deps = [
        ":data_java_lib",
    ],
)
