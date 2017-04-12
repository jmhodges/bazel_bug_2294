workspace(name = "bazel_bug_2294")

new_http_archive(
    name = "golang_linux_amd64",
    build_file_content = "",
    sha256 = "2e4dd6c44f0693bef4e7b46cc701513d74c3cc44f2419bf519d7868b12931ac3",
    strip_prefix = "go",
    url = "https://storage.googleapis.com/golang/go1.7.5.linux-amd64.tar.gz",
)

new_http_archive(
    name = "golang_darwin_amd64",
    build_file_content = "",
    sha256 = "2e2a5e0a5c316cf922cf7d59ee5724d49fc35b07a154f6c4196172adfc14b2ca",
    strip_prefix = "go",
    url = "https://storage.googleapis.com/golang/go1.7.5.darwin-amd64.tar.gz",
)

# new_http_archive(
#     name = "golang_linux_amd64",
#     build_file_content = "",
#     sha256 = "bb8fe0d81161e4a8b0a8b2145ee5f8a60370baf5d48c07a83f6f09e1ad253bec",
#     strip_prefix = "go",
#     url = "https://storage.googleapis.com/golang/go1.8rc1.linux-amd64.tar.gz",
# )

# new_http_archive(
#     name = "golang_darwin_amd64",
#     build_file_content = "",
#     sha256 = "faf2530afbc78d8fa64054960a130f10aa2b183abd5879cdfd2ec1a4bca01ff3",
#     strip_prefix = "go",
#     url = "https://storage.googleapis.com/golang/go1.8rc1.darwin-amd64.tar.gz",
# )

git_repository(
    name = "io_bazel_rules_go",
    remote = "https://github.com/bazelbuild/rules_go.git",
    tag = "0.4.3"
)

load("@io_bazel_rules_go//go:def.bzl", "go_repositories", "new_go_repository")

go_repositories(go_linux = "@golang_linux_amd64", go_darwin = "@golang_darwin_amd64")
