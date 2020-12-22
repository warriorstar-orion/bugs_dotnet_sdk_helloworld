load("@io_bazel_rules_dotnet//dotnet:defs.bzl", "net_binary", "core_binary")

core_binary(
    name = "core_a.exe",
    srcs = [
        "a.cs",
    ],
    deps =[ "@io_bazel_rules_dotnet//dotnet/stdlib:system.dll", ],
)

net_binary(
    name = "net_a.exe",
    srcs = [
        "a.cs",
    ],
    deps =[ "@io_bazel_rules_dotnet//dotnet/stdlib:system.dll", ],
)
