load("@npm//@bazel/typescript:index.bzl", "ts_project")

package(default_visibility = ["//visibility:public"])

ts_project(
    name = "types",
    srcs = glob(["**/*.ts"]),
    declaration = True,
    declaration_map = True,
    emit_declaration_only = True,
    tsconfig = "//:tsconfig",
    deps = [
        "//src/foo:types"
    ],
    args = [
        '--traceResolution'
    ]
)
