# testcase repository for Apache Maven invoker plugin, MINVOKER-317

See [MINVOKER-317](https://issues.apache.org/jira/browse/MINVOKER-317)

This bug exists at least until version 3.4.0

How to reproduce:

- clone this repository
- run  `mvn clean install`
  - the build succeeds and runs integration tests

- run `mvn -pl :test clean install`
  - one integration test fails

- run `mvn -am -pl :test clean install`
  - the build succeeds
