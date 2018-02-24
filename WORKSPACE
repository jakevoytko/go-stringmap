http_archive(
    name = "io_bazel_rules_go",
    sha256 = "53c8222c6eab05dd49c40184c361493705d4234e60c42c4cd13ab4898da4c6be",
    url = "https://github.com/bazelbuild/rules_go/releases/download/0.10.0/rules_go-0.10.0.tar.gz",
)

http_archive(
    name = "bazel_gazelle",
    sha256 = "6228d9618ab9536892aa69082c063207c91e777e51bd3c5544c9c060cafe1bd8",
    url = "https://github.com/bazelbuild/bazel-gazelle/releases/download/0.10.0/bazel-gazelle-0.10.0.tar.gz",
)

load("@io_bazel_rules_go//go:def.bzl", "go_rules_dependencies", "go_register_toolchains", "go_repository")

go_repository(
    name = "com_github_go_redis_redis",
    importpath = "github.com/go-redis/redis",
    tag = "v6.9.1",
)

go_rules_dependencies()

go_register_toolchains()

load("@bazel_gazelle//:deps.bzl", "gazelle_dependencies")

gazelle_dependencies()
