junit_tests(
    sources = globs(
        "com/twitter/inject/app/tests/*.scala",
        "com/twitter/inject/app/tests/internal/*.scala",
    ),
    compiler_option_sets = {"fatal_warnings"},
    dependencies = [
        ":test-deps",
        "3rdparty/jvm/com/google/inject:guice",
        "3rdparty/jvm/com/google/inject/extensions:guice-assistedinject",
        "3rdparty/jvm/com/google/inject/extensions:guice-multibindings",
        "3rdparty/jvm/com/google/inject/extensions:guice-testlib",
        "3rdparty/jvm/javax/inject:javax.inject",
        "3rdparty/jvm/junit",
        "3rdparty/jvm/net/codingwell:scala-guice",
        "3rdparty/jvm/org/scalatest",
        "3rdparty/jvm/org/slf4j:slf4j-api",
        "3rdparty/jvm/org/slf4j:slf4j-simple",
        "finatra/inject/inject-app/src/main/java",
        "finatra/inject/inject-app/src/main/scala",
        "finatra/inject/inject-app/src/test/java",
        "finatra/inject/inject-core/src/main/scala",
        "finatra/inject/inject-core/src/test/scala:test-deps",
        "finatra/inject/inject-slf4j/src/main/scala",
        "util/util-app/src/main/scala",
        "util/util-core/src/main/scala",
        "util/util-slf4j-api/src/main/scala",
    ],
)

scala_library(
    name = "test-deps",
    sources = globs(
        "com/twitter/inject/app/*.scala",
    ),
    compiler_option_sets = {"fatal_warnings"},
    provides = scala_artifact(
        org = "com.twitter",
        name = "inject-app-tests",
        repo = artifactory,
    ),
    dependencies = [
        "//:scala-reflect",
        "3rdparty/jvm/com/google/inject:guice",
        "3rdparty/jvm/com/google/inject/extensions:guice-assistedinject",
        "3rdparty/jvm/com/google/inject/extensions:guice-multibindings",
        "3rdparty/jvm/com/google/inject/extensions:guice-testlib",
        "3rdparty/jvm/net/codingwell:scala-guice",
        "3rdparty/jvm/org/slf4j:jcl-over-slf4j",
        "finatra/inject/inject-app/src/main/scala",
        "finatra/inject/inject-core/src/main/scala",
        "finatra/inject/inject-slf4j/src/main/scala",
        "util/util-app/src/main/scala",
        "util/util-slf4j-api/src/main/scala",
    ],
)
