# lux-hello-world

Compiling and running with the old compiler:

    lein-2.7.1 lux build && java -jar target/program.jar

succeeds and prints

    [COMPILATION BEGAN]
    Compilation complete!
    [COMPILATION ENDED]
    "Elapsed time: 5670.237296 msecs"
    [JVM PACKAGING BEGAN]
    [JVM PACKAGING ENDED]
    "Elapsed time: 1909.611654 msecs"
    Hello World!


Compiling with the new compiler:

    java -jar [path-to-new-compiler]/target/program.jar build --source source/ --target target/ --module program

fails with

    Compilation failed:
    {lux/tool/compiler/meta/io/context.cannot-find-module}
    Module: lux
