load("//tools:defs.bzl", "go_library")

package(licenses = ["notice"])

go_library(
    name = "dev",
    srcs = [
        "dev.go",
        "device.go",
        "fs.go",
        "full.go",
        "null.go",
        "random.go",
        "tty.go",
    ],
    visibility = ["//pkg/sentry:internal"],
    deps = [
        "//pkg/abi/linux",
        "//pkg/context",
        "//pkg/rand",
        "//pkg/safemem",
        "//pkg/sentry/device",
        "//pkg/sentry/fs",
        "//pkg/sentry/fs/fsutil",
        "//pkg/sentry/fs/ramfs",
        "//pkg/sentry/fs/tmpfs",
        "//pkg/sentry/memmap",
        "//pkg/sentry/mm",
        "//pkg/sentry/pgalloc",
        "//pkg/syserror",
        "//pkg/usermem",
        "//pkg/waiter",
    ],
)
