# hello-spring

This application is an example of using Spring MVC and Gradle.

## Usage

After cloning run.

```bash
gradle jettyRunWar
```

Visit [http://localhost:8080](http://localhost:8080).

## Additional Information

This repo is written about [here](https://github.com/scottmotte/writings/blob/master/articles/hello-world-with-spring-and-gradle.md).

## Deploying to Cloud Foundry

```bash
gem install cf
cf target api.run.pivotal.io
cf login
gradle assemble
cf push --path build/libs/hello-spring.war
```
