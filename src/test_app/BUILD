package(default_visibility = [])

subinclude("//:yarn")

filegroup(
    name = "src_files",
    srcs = glob([
        "public/**",
        "*.js",
        "src/*.js",
        "src/assets/**",
        "**/*.vue",
    ]),
)

yarn_install(name = "packages")

yarn_build(name = "dist",
           srcs=[":src_files"],
           deps=[":packages"])

