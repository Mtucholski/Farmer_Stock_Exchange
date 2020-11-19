
# JHipster Registry
 [JHipster](https://www.jhipster.tech/) registry service, which is based on:
  [Spring Cloud Netflix](https://cloud.spring.io/spring-cloud-netflix/), 
  [Eureka](https://github.com/Netflix/eureka) and
  [Spring Cloud Config](https://cloud.spring.io/spring-cloud-config/).

Full documentation: 
[JHipster documentation for microservices](https://www.jhipster.tech/microservices-architecture).

## Deploying to Heroku

[![Deploying to Heroku](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

 Some limitations when deploying to Heroku.

- The Jhipster registry work only with [native configuration](https://www.jhipster.tech/jhipster-registry/#spring-cloud-config) (and not Git config).
- The registry service cannot be scaled up to multiple dynos to provide redundancy. You must deploy multiple applications (i.e. click the button more than once). This is because Eureka requires distinct URLs to synchronize in-memory state between instances.

## Running locally

To run the cloned repository;

- For development run `./mvnw -Pdev,webpack` to just start in development or run `./mvnw` and run `npm install && npm start` for hot reload of client side code.
- For production profile run `./mvnw -Pprod`

[travis-image]: https://travis-ci.org/jhipster/jhipster-registry.svg?branch=master
[travis-url]: https://travis-ci.org/jhipster/jhipster-registry

