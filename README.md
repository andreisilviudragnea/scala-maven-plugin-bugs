# scala-maven-plugin-bugs

Run `./mvnw clean package`. It fails with:
```
[ERROR] Failed to execute goal net.alchim31.maven:scala-maven-plugin:4.5.6:compile (source-compile) on project scala-maven-plugin-bug: Execution source-compile of goal net.alchim31.maven:scala-maven-plugin:4.5.6:compile failed: A required class was missing while executing net.alchim31.maven:scala-maven-plugin:4.5.6:compile: scala/Function1
[ERROR] -----------------------------------------------------
[ERROR] realm =    plugin>net.alchim31.maven:scala-maven-plugin:4.5.6
[ERROR] strategy = org.codehaus.plexus.classworlds.strategy.SelfFirstStrategy
[ERROR] urls[0] = file:/Users/dragnea/.m2/repository/net/alchim31/maven/scala-maven-plugin/4.5.6/scala-maven-plugin-4.5.6.jar
[ERROR] urls[1] = file:/Users/dragnea/.m2/repository/org/apache/maven/shared/maven-dependency-tree/3.1.0/maven-dependency-tree-3.1.0.jar
[ERROR] urls[2] = file:/Users/dragnea/.m2/repository/org/sonatype/aether/aether-util/1.13.1/aether-util-1.13.1.jar
[ERROR] urls[3] = file:/Users/dragnea/.m2/repository/org/sonatype/sisu/sisu-inject-bean/2.3.0/sisu-inject-bean-2.3.0.jar
[ERROR] urls[4] = file:/Users/dragnea/.m2/repository/org/sonatype/sisu/sisu-guice/3.1.0/sisu-guice-3.1.0-no_aop.jar
[ERROR] urls[5] = file:/Users/dragnea/.m2/repository/org/sonatype/sisu/sisu-guava/0.9.9/sisu-guava-0.9.9.jar
[ERROR] urls[6] = file:/Users/dragnea/.m2/repository/org/codehaus/plexus/plexus-component-annotations/1.5.5/plexus-component-annotations-1.5.5.jar
[ERROR] urls[7] = file:/Users/dragnea/.m2/repository/org/sonatype/plexus/plexus-sec-dispatcher/1.3/plexus-sec-dispatcher-1.3.jar
[ERROR] urls[8] = file:/Users/dragnea/.m2/repository/org/sonatype/plexus/plexus-cipher/1.4/plexus-cipher-1.4.jar
[ERROR] urls[9] = file:/Users/dragnea/.m2/repository/org/eclipse/aether/aether-util/1.1.0/aether-util-1.1.0.jar
[ERROR] urls[10] = file:/Users/dragnea/.m2/repository/org/apache/maven/reporting/maven-reporting-api/3.0/maven-reporting-api-3.0.jar
[ERROR] urls[11] = file:/Users/dragnea/.m2/repository/org/apache/maven/doxia/doxia-sink-api/1.0/doxia-sink-api-1.0.jar
[ERROR] urls[12] = file:/Users/dragnea/.m2/repository/org/apache/maven/maven-archiver/3.5.1/maven-archiver-3.5.1.jar
[ERROR] urls[13] = file:/Users/dragnea/.m2/repository/org/apache/maven/shared/maven-shared-utils/3.3.3/maven-shared-utils-3.3.3.jar
[ERROR] urls[14] = file:/Users/dragnea/.m2/repository/commons-io/commons-io/2.6/commons-io-2.6.jar
[ERROR] urls[15] = file:/Users/dragnea/.m2/repository/org/codehaus/plexus/plexus-interpolation/1.26/plexus-interpolation-1.26.jar
[ERROR] urls[16] = file:/Users/dragnea/.m2/repository/org/apache/commons/commons-exec/1.3/commons-exec-1.3.jar
[ERROR] urls[17] = file:/Users/dragnea/.m2/repository/org/codehaus/plexus/plexus-utils/3.4.1/plexus-utils-3.4.1.jar
[ERROR] urls[18] = file:/Users/dragnea/.m2/repository/org/codehaus/plexus/plexus-archiver/4.2.6/plexus-archiver-4.2.6.jar
[ERROR] urls[19] = file:/Users/dragnea/.m2/repository/org/codehaus/plexus/plexus-io/3.2.0/plexus-io-3.2.0.jar
[ERROR] urls[20] = file:/Users/dragnea/.m2/repository/org/apache/commons/commons-compress/1.21/commons-compress-1.21.jar
[ERROR] urls[21] = file:/Users/dragnea/.m2/repository/org/iq80/snappy/snappy/0.4/snappy-0.4.jar
[ERROR] urls[22] = file:/Users/dragnea/.m2/repository/org/tukaani/xz/1.9/xz-1.9.jar
[ERROR] urls[23] = file:/Users/dragnea/.m2/repository/org/scala-sbt/zinc_2.13/1.5.8/zinc_2.13-1.5.8.jar
[ERROR] urls[24] = file:/Users/dragnea/.m2/repository/org/scala-lang/scala-library/2.13.6/scala-library-2.13.6.jar
[ERROR] urls[25] = file:/Users/dragnea/.m2/repository/org/scala-sbt/zinc-core_2.13/1.5.8/zinc-core_2.13-1.5.8.jar
[ERROR] urls[26] = file:/Users/dragnea/.m2/repository/org/scala-sbt/zinc-apiinfo_2.13/1.5.8/zinc-apiinfo_2.13-1.5.8.jar
[ERROR] urls[27] = file:/Users/dragnea/.m2/repository/org/scala-sbt/compiler-bridge_2.13/1.5.8/compiler-bridge_2.13-1.5.8.jar
[ERROR] urls[28] = file:/Users/dragnea/.m2/repository/org/scala-sbt/zinc-classpath_2.13/1.5.8/zinc-classpath_2.13-1.5.8.jar
[ERROR] urls[29] = file:/Users/dragnea/.m2/repository/org/scala-lang/scala-compiler/2.13.6/scala-compiler-2.13.6.jar
[ERROR] urls[30] = file:/Users/dragnea/.m2/repository/org/scala-sbt/compiler-interface/1.5.8/compiler-interface-1.5.8.jar
[ERROR] urls[31] = file:/Users/dragnea/.m2/repository/org/scala-sbt/util-interface/1.5.6/util-interface-1.5.6.jar
[ERROR] urls[32] = file:/Users/dragnea/.m2/repository/org/scala-sbt/zinc-persist-core-assembly/1.5.8/zinc-persist-core-assembly-1.5.8.jar
[ERROR] urls[33] = file:/Users/dragnea/.m2/repository/org/scala-lang/modules/scala-parallel-collections_2.13/0.2.0/scala-parallel-collections_2.13-0.2.0.jar
[ERROR] urls[34] = file:/Users/dragnea/.m2/repository/org/scala-sbt/io_2.13/1.5.1/io_2.13-1.5.1.jar
[ERROR] urls[35] = file:/Users/dragnea/.m2/repository/com/swoval/file-tree-views/2.1.6/file-tree-views-2.1.6.jar
[ERROR] urls[36] = file:/Users/dragnea/.m2/repository/net/java/dev/jna/jna/5.5.0/jna-5.5.0.jar
[ERROR] urls[37] = file:/Users/dragnea/.m2/repository/net/java/dev/jna/jna-platform/5.5.0/jna-platform-5.5.0.jar
[ERROR] urls[38] = file:/Users/dragnea/.m2/repository/org/scala-sbt/util-logging_2.13/1.5.6/util-logging_2.13-1.5.6.jar
[ERROR] urls[39] = file:/Users/dragnea/.m2/repository/org/scala-sbt/collections_2.13/1.5.6/collections_2.13-1.5.6.jar
[ERROR] urls[40] = file:/Users/dragnea/.m2/repository/org/scala-sbt/util-position_2.13/1.5.6/util-position_2.13-1.5.6.jar
[ERROR] urls[41] = file:/Users/dragnea/.m2/repository/org/scala-sbt/core-macros_2.13/1.5.6/core-macros_2.13-1.5.6.jar
[ERROR] urls[42] = file:/Users/dragnea/.m2/repository/org/jline/jline-terminal/3.19.0/jline-terminal-3.19.0.jar
[ERROR] urls[43] = file:/Users/dragnea/.m2/repository/org/scala-lang/scala-reflect/2.13.6/scala-reflect-2.13.6.jar
[ERROR] urls[44] = file:/Users/dragnea/.m2/repository/org/scala-sbt/util-relation_2.13/1.5.6/util-relation_2.13-1.5.6.jar
[ERROR] urls[45] = file:/Users/dragnea/.m2/repository/org/scala-sbt/zinc-persist_2.13/1.5.8/zinc-persist_2.13-1.5.8.jar
[ERROR] urls[46] = file:/Users/dragnea/.m2/repository/org/scala-sbt/zinc-compile-core_2.13/1.5.8/zinc-compile-core_2.13-1.5.8.jar
[ERROR] urls[47] = file:/Users/dragnea/.m2/repository/org/scala-lang/modules/scala-parser-combinators_2.13/1.1.2/scala-parser-combinators_2.13-1.1.2.jar
[ERROR] urls[48] = file:/Users/dragnea/.m2/repository/net/openhft/zero-allocation-hashing/0.10.1/zero-allocation-hashing-0.10.1.jar
[ERROR] urls[49] = file:/Users/dragnea/.m2/repository/org/scala-sbt/util-control_2.13/1.5.6/util-control_2.13-1.5.6.jar
[ERROR] urls[50] = file:/Users/dragnea/.m2/repository/org/scala-sbt/zinc-classfile_2.13/1.5.8/zinc-classfile_2.13-1.5.8.jar
[ERROR] Number of foreign imports: 1
[ERROR] import: Entry[import  from realm ClassRealm[maven.api, parent: null]]
[ERROR] 
[ERROR] -----------------------------------------------------
[ERROR] : scala.Function1
[ERROR] -> [Help 1]
[ERROR] 
[ERROR] To see the full stack trace of the errors, re-run Maven with the -e switch.
[ERROR] Re-run Maven using the -X switch to enable full debug logging.
[ERROR] 
[ERROR] For more information about the errors and possible solutions, please read the following articles:
[ERROR] [Help 1] http://cwiki.apache.org/confluence/display/MAVEN/PluginContainerException
```

Change `<scala.version.minor>8</scala.version.minor>` to `<scala.version.minor>7</scala.version.minor>`,
run `./mvnw clean package` and the build completes successfully.

Output of `java -version`:
```
openjdk version "11.0.14" 2022-01-18 LTS
OpenJDK Runtime Environment Corretto-11.0.14.9.1 (build 11.0.14+9-LTS)
OpenJDK 64-Bit Server VM Corretto-11.0.14.9.1 (build 11.0.14+9-LTS, mixed mode)
```

Output of `uname -a`:
```
Darwin MacBook-Pro-5.local 21.3.0 Darwin Kernel Version 21.3.0: Wed Jan  5 21:37:58 PST 2022; root:xnu-8019.80.24~20/RELEASE_X86_64 x86_64
```
