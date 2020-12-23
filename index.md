---
layout: default
---

- By executing Lerna's scripts to VMs running on the cloud (public or private), you can build an environment that is configured to achieve high availability and high throughput.
- In that environment, designing and implementing applications based on the actor model ([Akka](https://akka.io/)) and CQRS(Command Query Responsibility Segregation) with Event Sourcing architecture allows you to build highly available systems.
- Libraries and reference implementations for design and implementation are provided.


![](img/lerna_overview.png)


## Concept

### High availability and high throughput

- Eliminates the bottleneck of writing to the RDBMS by applying the CQRS with Event Sourcing architecture to the application layer
- High Availability and Scalability with Akka Cluster
- Provides responsiveness by making the application stateful, while providing fast failover with guaranteed consistency using Raft

### Platform independent

- Fast failover at the middleware and application layers with platform independence, based on the premise that the server (VM) will stop.
- This ensures high availability independent of hardware and specific cloud environments


### Low cost and fast delivery

- No need to purchase expensive high-availability servers; high availability can be achieved at low cost by using OSS middleware.
- Because it can be built on the cloud, it reduces the lead time for hardware procurement and improves delivery speed.


## Contents
![](img/lerna_content_map.png)

| Name  | Description |
| ----------- | ---- |
| [lerna.g8](https://github.com/lerna-stack/lerna.g8) | templete for createing a new project |
| [lerna-terraform](https://github.com/lerna-stack/lerna-terraform) | scripts to build the environment |
| [lerna-sample-payment-app](https://github.com/lerna-stack/lerna-sample-payment-app)  | sample applications for developing with Lerna |
| [lerna-design](https://github.com/lerna-stack/lerna-design) | documentation for developing with Lerna |
| Learning Content | Coming soon. |
| lerna-sample-batch-app | Coming soon. |

## Libraries
- [Lerna API](scaladoc/index.html)

| Name  | Description |
| ----------- | ---- |
| [akka-entity-replication](https://github.com/lerna-stack/akka-entity-replication) | Akka extension for fast recovery from failure with replicating stateful entity on multiple nodes in Cluster. |
| [lerna-http](https://github.com/lerna-stack/lerna-app-library/blob/main/doc/lerna-http.md) | Lerna HTTP library provides HTTP related features like below.<br> - Custom Json Format for [spray-json](https://github.com/spray/spray-json) <br> - Custom Directives for [Akka HTTP](https://doc.akka.io/docs/akka-http/current/index.html) <br> - Custom Header for [Akka HTTP](https://doc.akka.io/docs/akka-http/current/index.html) |
| [lerna-log](https://github.com/lerna-stack/lerna-app-library/blob/main/doc/lerna-log.md) | Lerna Log library provides logging related features like below. <br> - Custom log converters for [Logback](http://logback.qos.ch/) |
| [lerna-management](https://github.com/lerna-stack/lerna-app-library/blob/main/doc/lerna-management.md) | Lerna Management library provides management related features like below. <br> - SNMP metrics provider for [Kamon](https://kamon.io/) |
| [lerna-testkit](https://github.com/lerna-stack/lerna-app-library/blob/main/doc/lerna-testkit.md) | Lerna TestKit library provides testkits for <br> - [Akka Classic](https://doc.akka.io/docs/akka/current/index-classic.html) <br> - [Airframe](https://wvlet.org/airframe/) <br> - [WireMock](http://wiremock.org/~~~~) |
| [lerna-util](https://github.com/lerna-stack/lerna-app-library/blob/main/doc/lerna-util.md) | Lerna Util library provides some utilities like below. <br> - Encryption <br> - Typed Equals <br> - Security <br> - Date and Time |
| [lerna-util-akka](https://github.com/lerna-stack/lerna-app-library/blob/main/doc/lerna-util-akka.md) | Lerna Util Akka library provides some utilities related Akka Classic. |
| [lerna-util-sequence](https://github.com/lerna-stack/lerna-app-library/blob/main/doc/lerna-util-sequence.md) | Lerna Util Sequence library provides an ID generator. | 
| [lerna-validation](https://github.com/lerna-stack/lerna-app-library/blob/main/doc/lerna-validation.md) | Lerna Validation library provides custom validators for [Accord](http://wix.github.io/accord/). |
| [lerna-wart-core](https://github.com/lerna-stack/lerna-app-library/blob/main/doc/lerna-wart-core.md) | Lerna Wart Core library provides custom warts for [WartRemover](https://www.wartremover.org/) |
| nablarch-fw-batch-parallelizable | Coming soon! |

## Getting started

### Running on your local machine
- see [lerna-sample-payment-app](https://github.com/lerna-stack/lerna-sample-payment-app)

### Running on your server
- see [lerna-terraform](https://github.com/lerna-stack/lerna-terraform)

### Local development
- see [lerna.g8](https://github.com/lerna-stack/lerna.g8)
- create blank project executing `sbt new lerna-stack/lerna.g8`

## License
Lerna is released under the terms of the [Apache License Version 2.0](./LICENSE).

<!-- Escape to set blank lines and use "*" -->
\
\
\* The names of the companies and products described in this site are trademarks or registered trademarks of the respective companies.  
\* Amazon Web Services, AWS are trademarks of Amazon.com, Inc. or its affiliates in the United States and/or other countries.  
\* Akka is a trademark of Lightbend, Inc.


© 2020 TIS Inc.


<div>
<!-- Global site tag (gtag.js) - Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=UA-179004683-1"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'UA-179004683-1');
</script>
</div>