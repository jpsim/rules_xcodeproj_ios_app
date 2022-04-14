load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "com_github_buildbuddy_io_rules_xcodeproj",
    sha256 = "f8ab5d6d57fc87a03cc297b6417a2c75c280a3abdf17a05b27a3dcab4c20d787",
    strip_prefix = "rules_xcodeproj-55142f56245dd411c560862306e77379ac71bbd8",
    url = "https://github.com/buildbuddy-io/rules_xcodeproj/archive/55142f56245dd411c560862306e77379ac71bbd8.tar.gz",
)

load(
    "@com_github_buildbuddy_io_rules_xcodeproj//xcodeproj:repositories.bzl",
    "xcodeproj_rules_dependencies",
)

xcodeproj_rules_dependencies()

load(
    "@build_bazel_rules_apple//apple:repositories.bzl",
    "apple_rules_dependencies",
)

apple_rules_dependencies()

load(
    "@build_bazel_rules_swift//swift:repositories.bzl",
    "swift_rules_dependencies",
)

swift_rules_dependencies()

load(
    "@build_bazel_rules_swift//swift:extras.bzl",
    "swift_rules_extra_dependencies",
)

swift_rules_extra_dependencies()

load(
    "@build_bazel_apple_support//lib:repositories.bzl",
    "apple_support_dependencies",
)

apple_support_dependencies()
