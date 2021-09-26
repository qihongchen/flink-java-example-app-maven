# flink-java-example-app-maven

A Flink word count example application in Java with Maven build. You can use this as the start point for your flink java application.

### Add new dependency

Add new dependency like following in `dependencies` section, this dependency will be included
in the final uber/fat jar.
```
<dependency>
	<groupId>org.apache.flink</groupId>
	<artifactId>flink-connector-kafka_${scala.binary.version}</artifactId>
	<version>${flink.version}</version>
</dependency>
```

### Build

```
 mvn clean package
```


The final uber/fat jar is in `target` directory, something like `target/flink-example-app-wordcount-0.1.jar`.

### Reference

[Flink Application Maven Quick start](https://nightlies.apache.org/flink/flink-docs-release-1.13/docs/dev/datastream/project-configuration/#maven-quickstart)

The example WordCount source code is from Apache Flink Project.