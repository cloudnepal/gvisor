load("//tools:defs.bzl", "go_binary")

package(
    default_applicable_licenses = ["//:license"],
    licenses = ["notice"],
)

go_binary(
    name = "tun_tcp_echo",
    srcs = ["main.go"],
    visibility = ["//:sandbox"],
    deps = [
        "//pkg/rawfile",
        "//pkg/tcpip",
        "//pkg/tcpip/link/fdbased",
        "//pkg/tcpip/link/tun",
        "//pkg/tcpip/network/arp",
        "//pkg/tcpip/network/ipv4",
        "//pkg/tcpip/network/ipv6",
        "//pkg/tcpip/stack",
        "//pkg/tcpip/transport/tcp",
        "//pkg/waiter",
    ],
)
