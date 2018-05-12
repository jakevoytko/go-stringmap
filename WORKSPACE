http_archive(
    name = "io_bazel_rules_go",
    sha256 = "c1f52b8789218bb1542ed362c4f7de7052abcf254d865d96fb7ba6d44bc15ee3",
    url = "https://github.com/bazelbuild/rules_go/releases/download/0.12.0/rules_go-0.12.0.tar.gz",
)

http_archive(
    name = "bazel_gazelle",
    sha256 = "92a3c59734dad2ef85dc731dbcb2bc23c4568cded79d4b87ebccd787eb89e8d0",
    url = "https://github.com/bazelbuild/bazel-gazelle/releases/download/0.12.0/bazel-gazelle-0.12.0.tar.gz",
)

load("@io_bazel_rules_go//go:def.bzl", "go_rules_dependencies", "go_register_toolchains", "go_repository")

go_repository(
    name = "com_github_go_redis_redis",
    importpath = "github.com/go-redis/redis",
    tag = "v6.10.2",
)

go_rules_dependencies()

go_register_toolchains()

load("@bazel_gazelle//:deps.bzl", "gazelle_dependencies")

gazelle_dependencies()
