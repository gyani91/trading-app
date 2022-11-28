# Simple Trading Application

This is a simple trading application.

## Required tools and libraries

1. [JDK 19](https://www.oracle.com/java/technologies/downloads/#JDK19)
2. At least [Maven 3.6.3](https://maven.apache.org/download.cgi)

## Build the code

Execute in a shell

```shell
git clone https://github.com/gyani91/trading-app.git
cd trading-app
mvn -U clean verify -DskipTests
```

Note: here tests are skipped, since they are executed later, see the Chapter
"Test the code".

In this way, a new jar file will be created in the `target` folder, e.g.
`target/trading-0.0.2-SNAPSHOT.jar`.

## Run the code

```shell
java -jar target/trading-0.0.2-SNAPSHOT.jar
```

## Test the code

Once you launched the main application, you can test it as

```shell
export CUCUMBER_PUBLISH_TOKEN=876b2396-60aa-4b20-b78b-a584427556bd
mvn test
```

## Check the report

You get the run report directly on the terminal and the same report is also
published to the following [collection](https://reports.cucumber.io/report-collections/ddd94d0f-88ab-49ea-8040-f73cf824ab2b).
