load("@build_bazel_rules_apple//apple:ios.bzl", "ios_application")
load("@build_bazel_rules_swift//swift:swift.bzl", "swift_library")

ios_application(
    name = "Example",
    app_icons = glob(["Assets.xcassets/AppIcon.appiconset/**"]),
    bundle_id = "io.buildbuddy.example",
    bundle_name = "Example",
    families = ["iphone"],
    infoplists = [":Info.plist"],
    minimum_os_version = "15.0",
    visibility = ["//visibility:public"],
    deps = [":Example.library"],
)

swift_library(
    name = "Example.library",
    srcs = glob(["**/*.swift"]),
    module_name = "Example",
    tags = ["manual"],
    visibility = ["//visibility:public"],
    deps = [],
)
