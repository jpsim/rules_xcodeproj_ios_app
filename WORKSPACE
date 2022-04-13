load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

# This fails with errors like:
# "Unable to load contents of file list: 'iOS App.xcodeproj/rules_xcodeproj/modulemaps.fixed.xcfilelist'
http_archive(
    name = "com_github_buildbuddy_io_rules_xcodeproj",
    sha256 = "e82b24c55e479905383d1567d7617a14d1995638bf78b468218f7a44c176ce15",
    url = "https://github.com/buildbuddy-io/rules_xcodeproj/archive/8449a6e913633a4a15d7819a6a614ca2c17e4338.tar.gz",
)

# This works when rules_xcodeproj is checked out next to this example
# local_repository(
#     name = "com_github_buildbuddy_io_rules_xcodeproj",
#     path = "../rules_xcodeproj",
# )

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
