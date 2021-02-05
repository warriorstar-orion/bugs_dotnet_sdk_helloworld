load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "io_bazel_rules_dotnet",
    url = "https://github.com/bazelbuild/rules_dotnet/archive/0.0.6.zip",
    strip_prefix = "rules_dotnet-0.0.6",
)

load("@io_bazel_rules_dotnet//dotnet:deps.bzl", "dotnet_repositories")

dotnet_repositories()

load("@io_bazel_rules_dotnet//dotnet:defs.bzl", "core_register_sdk", 
    "dotnet_register_toolchains", "dotnet_repositories_nugets")

dotnet_register_toolchains()
dotnet_repositories_nugets()
core_register_sdk(name="core_sdk")