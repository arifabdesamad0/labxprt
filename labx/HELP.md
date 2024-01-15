# Getting Started

### Reference Documentation

For further reference, please consider the following sections:

* [Official Gradle documentation](https://docs.gradle.org)
* [Spring Boot Gradle Plugin Reference Guide](https://docs.spring.io/spring-boot/docs/3.2.1/gradle-plugin/reference/html/)
* [Create an OCI image](https://docs.spring.io/spring-boot/docs/3.2.1/gradle-plugin/reference/html/#build-image)
* [Spring Boot DevTools](https://docs.spring.io/spring-boot/docs/3.2.1/reference/htmlsingle/index.html#using.devtools)
* [Apache Freemarker](https://docs.spring.io/spring-boot/docs/3.2.1/reference/htmlsingle/index.html#web.servlet.spring-mvc.template-engines)
* [Spring Web](https://docs.spring.io/spring-boot/docs/3.2.1/reference/htmlsingle/index.html#web)
* [Hilla](https://hilla.dev/)
* [Spring Configuration Processor](https://docs.spring.io/spring-boot/docs/3.2.1/reference/htmlsingle/index.html#appendix.configuration-metadata.annotation-processor)
* [Spring Reactive Web](https://docs.spring.io/spring-boot/docs/3.2.1/reference/htmlsingle/index.html#web.reactive)
* [Spring Web Services](https://docs.spring.io/spring-boot/docs/3.2.1/reference/htmlsingle/index.html#io.webservices)
* [Vaadin](https://vaadin.com/docs)
* [Spring Data JPA](https://docs.spring.io/spring-boot/docs/3.2.1/reference/htmlsingle/index.html#data.sql.jpa-and-spring-data)
* [Okta Spring Boot documentation](https://github.com/okta/okta-spring-boot#readme)
* [Spring Security](https://docs.spring.io/spring-boot/docs/3.2.1/reference/htmlsingle/index.html#web.security)
* [Rest Repositories](https://docs.spring.io/spring-boot/docs/3.2.1/reference/htmlsingle/index.html#howto.data-access.exposing-spring-data-repositories-as-rest)
* [Thymeleaf](https://docs.spring.io/spring-boot/docs/3.2.1/reference/htmlsingle/index.html#web.servlet.spring-mvc.template-engines)
* [Jersey](https://docs.spring.io/spring-boot/docs/3.2.1/reference/htmlsingle/index.html#web.servlet.jersey)
* [Spring Session](https://docs.spring.io/spring-session/reference/)
* [Spring LDAP](https://docs.spring.io/spring-boot/docs/3.2.1/reference/htmlsingle/index.html#data.nosql.ldap)
* [OAuth2 Client](https://docs.spring.io/spring-boot/docs/3.2.1/reference/htmlsingle/index.html#web.security.oauth2.client)
* [OAuth2 Resource Server](https://docs.spring.io/spring-boot/docs/3.2.1/reference/htmlsingle/index.html#web.security.oauth2.server)
* [Spring HATEOAS](https://docs.spring.io/spring-boot/docs/3.2.1/reference/htmlsingle/index.html#web.spring-hateoas)
* [OAuth2 Authorization Server](https://docs.spring.io/spring-boot/docs/3.2.1/reference/htmlsingle/index.html#web.security.oauth2.authorization-server)
* [Groovy Templates](https://docs.spring.io/spring-boot/docs/3.2.1/reference/htmlsingle/index.html#web.servlet.spring-mvc.template-engines)
* [Mustache](https://docs.spring.io/spring-boot/docs/3.2.1/reference/htmlsingle/index.html#web.servlet.spring-mvc.template-engines)
* [Spring Data JDBC](https://docs.spring.io/spring-boot/docs/3.2.1/reference/htmlsingle/index.html#data.sql.jdbc)
* [Spring for GraphQL](https://docs.spring.io/spring-boot/docs/3.2.1/reference/htmlsingle/index.html#web.graphql)

### Guides

The following guides illustrate how to use some features concretely:

* [Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/)
* [Serving Web Content with Spring MVC](https://spring.io/guides/gs/serving-web-content/)
* [Building REST services with Spring](https://spring.io/guides/tutorials/rest/)
* [Next Steps with Hilla](https://hilla.dev/docs/react/start/quick/#coming-from-spring-initializr)
* [Building a Reactive RESTful Web Service](https://spring.io/guides/gs/reactive-rest-service/)
* [Producing a SOAP web service](https://spring.io/guides/gs/producing-web-service/)
* [Creating CRUD UI with Vaadin](https://spring.io/guides/gs/crud-with-vaadin/)
* [Accessing Data with JPA](https://spring.io/guides/gs/accessing-data-jpa/)
* [Okta-Hosted Login Page Example](https://github.com/okta/samples-java-spring/tree/master/okta-hosted-login)
* [Custom Login Page Example](https://github.com/okta/samples-java-spring/tree/master/custom-login)
* [Okta Spring Security Resource Server Example](https://github.com/okta/samples-java-spring/tree/master/resource-server)
* [Securing a Web Application](https://spring.io/guides/gs/securing-web/)
* [Spring Boot and OAuth2](https://spring.io/guides/tutorials/spring-boot-oauth2/)
* [Authenticating a User with LDAP](https://spring.io/guides/gs/authenticating-ldap/)
* [Accessing JPA Data with REST](https://spring.io/guides/gs/accessing-data-rest/)
* [Accessing Neo4j Data with REST](https://spring.io/guides/gs/accessing-neo4j-data-rest/)
* [Accessing MongoDB Data with REST](https://spring.io/guides/gs/accessing-mongodb-data-rest/)
* [Handling Form Submission](https://spring.io/guides/gs/handling-form-submission/)
* [Building a Hypermedia-Driven RESTful Web Service](https://spring.io/guides/gs/rest-hateoas/)
* [Using Spring Data JDBC](https://github.com/spring-projects/spring-data-examples/tree/master/jdbc/basics)
* [Building a GraphQL service](https://spring.io/guides/gs/graphql-server/)

### Additional Links

These additional references should also help you:

* [Gradle Build Scans – insights for your project's build](https://scans.gradle.com#gradle)

## OAuth 2.0 and OIDC with Okta

If you don't have a free Okta developer account, you can create one with [the Okta CLI](https://cli.okta.com):

```bash
$ okta register
```

Then, register your Spring Boot app on Okta using:

```bash
$ okta apps create
```

Select **Web** > **Okta Spring Boot Starter** and accept the default redirect URIs.

## GraphQL code generation with DGS

This project has been configured to use the Netflix DGS Codegen plugin.
This plugin can be used to generate client files for accessing remote GraphQL services.
The default setup assumes that the GraphQL schema file for the remote service is added to
the `src/main/resources/graphql-client/` location.

You can learn more about
the [plugin configuration options](https://netflix.github.io/dgs/generating-code-from-schema/#configuring-code-generation)
and
[how to use the generated types](https://netflix.github.io/dgs/generating-code-from-schema/) to adapt the default setup.


