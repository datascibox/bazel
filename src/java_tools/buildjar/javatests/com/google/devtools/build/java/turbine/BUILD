filegroup(
    name = "srcs",
    srcs = glob(["**"]) + ["//src/java_tools/buildjar/javatests/com/google/devtools/build/java/turbine/javac:srcs"],
    visibility = ["//src/java_tools/buildjar:__pkg__"],
)

package_group(
    name = "packages",
    packages = ["//src/java_tools/buildjar/..."],
)

package(default_visibility = [":packages"])

java_test(
    name = "TurbineOptionsTest",
    srcs = ["TurbineOptionsTest.java"],
    tags = ["jdk8"],
    deps = [
        "//src/java_tools/buildjar/java/com/google/devtools/build/buildjar:JarOwner",
        "//src/java_tools/buildjar/java/com/google/devtools/build/java/turbine:turbine_options",
        "//src/java_tools/buildjar/java/com/google/devtools/build/java/turbine:turbine_options_parser",
        "//third_party:guava",
        "//third_party:junit4",
        "//third_party:truth",
    ],
)
