load("//tools:defs.bzl", "go_library")

package(licenses = ["notice"])

go_library(
    name = "control",
    srcs = ["control.go"],
    imports = [
        "gvisor.dev/gvisor/pkg/sentry/fs",
    ],
    visibility = ["//pkg/sentry:internal"],
    deps = [
        "//pkg/abi/linux",
        "//pkg/binary",
        "//pkg/context",
        "//pkg/sentry/fs",
        "//pkg/sentry/kernel",
        "//pkg/sentry/kernel/auth",
        "//pkg/sentry/socket",
        "//pkg/sentry/socket/unix/transport",
        "//pkg/syserror",
        "//pkg/usermem",
    ],
)
