load("//tools:defs.bzl", "go_library", "proto_library")

package(licenses = ["notice"])

go_library(
    name = "arch",
    srcs = [
        "aligned.go",
        "arch.go",
        "arch_aarch64.go",
        "arch_amd64.go",
        "arch_amd64.s",
        "arch_arm64.go",
        "arch_state_aarch64.go",
        "arch_state_x86.go",
        "arch_x86.go",
        "auxv.go",
        "signal.go",
        "signal_act.go",
        "signal_amd64.go",
        "signal_arm64.go",
        "signal_info.go",
        "signal_stack.go",
        "stack.go",
        "syscalls_amd64.go",
        "syscalls_arm64.go",
    ],
    visibility = ["//:sandbox"],
    deps = [
        ":registers_go_proto",
        "//pkg/abi/linux",
        "//pkg/binary",
        "//pkg/context",
        "//pkg/cpuid",
        "//pkg/log",
        "//pkg/sentry/limits",
        "//pkg/sync",
        "//pkg/syserror",
        "//pkg/usermem",
    ],
)

proto_library(
    name = "registers",
    srcs = ["registers.proto"],
    visibility = ["//visibility:public"],
)
