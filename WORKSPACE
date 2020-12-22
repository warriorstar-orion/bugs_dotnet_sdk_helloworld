load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "io_bazel_rules_dotnet",
    url = "https://github.com/bazelbuild/rules_dotnet/archive/98cc58708e0ea150a8737e7f83a74f0f41ececf8.zip",
     sha256 = "e5111d87a0a1a483a4a992fac860ea930b294ff8331b58a083b6fbaf4f6d31ec",
    strip_prefix = "rules_dotnet-98cc58708e0ea150a8737e7f83a74f0f41ececf8",
)

load("@io_bazel_rules_dotnet//dotnet:deps.bzl", "dotnet_repositories")

dotnet_repositories()

load("@io_bazel_rules_dotnet//dotnet:defs.bzl", "core_register_sdk", "net_register_sdk", "mono_register_sdk",
    "dotnet_register_toolchains", "dotnet_repositories_nugets", "nuget_package")

dotnet_register_toolchains()
dotnet_repositories_nugets()
core_register_sdk(name="dotnet_sdk")
net_register_sdk(name="net_sdk")