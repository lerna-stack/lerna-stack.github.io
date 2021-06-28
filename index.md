---
layout: default
---

- By executing Lerna's scripts to VMs running on the cloud (public or private), you can build an environment that is configured to achieve high availability and high throughput.
- In that environment, designing and implementing applications based on the actor model ([Akka](https://akka.io/)) and CQRS(Command Query Responsibility Segregation) with Event Sourcing architecture allows you to build highly available systems.
- Libraries and reference implementations for design and implementation are provided.


<object type="image/svg+xml" data="https://cdn.jsdelivr.net/gh/lerna-stack/lerna-stack.github.io@master/img/lerna_overview_en.drawio.svg"></object>


## Concept

### High availability and high throughput

- Eliminates the bottleneck of writing to the RDBMS by applying the CQRS with Event Sourcing architecture to the application layer
- High Availability and Scalability with Akka Cluster
- Provides responsiveness by making the application stateful, while providing fast failover with guaranteed consistency using Raft


<object type="image/svg+xml" data="https://cdn.jsdelivr.net/gh/lerna-stack/lerna-stack.github.io@master/img/benchmarkscore_en.drawio.svg"></object>


* Benchmark test report of Lerna available here(coming soon)

### Platform independent

- Fast failover at the middleware and application layers with platform independence, based on the premise that the server (VM) will stop.
- This ensures high availability independent of hardware and specific cloud environments


### Low cost and fast delivery

- No need to purchase expensive high-availability servers; high availability can be achieved at low cost by using OSS middleware.
- Because it can be built on the cloud, it reduces the lead time for hardware procurement and improves delivery speed.


## Contents

<object type="image/svg+xml" data="https://cdn.jsdelivr.net/gh/lerna-stack/lerna-stack.github.io@master/img/lerna_content_list_en.drawio.svg"></object>


| Name  | Description |
| ----------- | ---- |
| [application template](https://github.com/lerna-stack/lerna.g8) | a template for creating a new project |
| [Terraform scripts](https://github.com/lerna-stack/lerna-terraform) | scripts to build the environment |
| [learning content](https://github.com/lerna-stack/lerna-handson) | hands-on content learning Akka and Scala with Lerna |
| [system design documents](https://github.com/lerna-stack/lerna-design) | documentation for developing with Lerna |
| [application libraries](#application-libraries) | libraries for developing applications that run on Lerna Stack ( [API Doc](https://lerna-stack.github.io/scaladoc/index.html) ) |
| [sample application](https://github.com/lerna-stack/lerna-sample-payment-app)  | a sample application for developing with Lerna application libraries |
| [HA library](https://github.com/lerna-stack/akka-entity-replication) | Akka extension for fast recovery from failure with replicating stateful entity on multiple nodes in Cluster.  ( [API Doc](https://lerna-stack.github.io/akka-entity-replication/latest/api/) )|
| [ benchmark report for Lerna](https://fintan.jp/?p=5946) | a benchmark report measuring availability and throughput of Lerna |
| [sample application for HA library](https://github.com/lerna-stack/akka-entity-replication-sample)  | a sample application for developing with [HA library](https://github.com/lerna-stack/akka-entity-replication) |
| [batch parallelization library](https://github.com/lerna-stack/nablarch-fw-batch-parallelizable) | a library for parallelizing batch processing with [Nablarch Batch Framework](https://nablarch.github.io/docs/LATEST/doc/application_framework/application_framework/batch/index.html) |
| [ sample application for batch library](https://github.com/lerna-stack/nablarch-fw-batch-parallelizable-example) | a sample application for developing with [batch parallelization library](https://github.com/lerna-stack/nablarch-fw-batch-parallelizable) |
| [ benchmark report for batch library](https://fintan.jp/?p=7061) | a report testing speed improvement effect by parallelizing processing using [batch parallelization library](https://github.com/lerna-stack/nablarch-fw-batch-parallelizable) |


## Getting started

<object type="image/svg+xml" data="https://cdn.jsdelivr.net/gh/lerna-stack/lerna-stack.github.io@master/img/getting_started_en.drawio.svg"></object>


## Articles

- [Does parallelizing batch processing in Lerna make it linearly faster? (Fintan)](https://fintan.jp/?p=7061)
- [The paradigm of the many-core era; Learn about reactive systems. (ThinkIT)](https://thinkit.co.jp/series/5659)

## Slides

<iframe src="//www.slideshare.net/slideshow/embed_code/key/z5PCknVjHaFfxz" width="510" height="420" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen> </iframe> <div style="margin-bottom:5px"> <strong> <a href="//www.slideshare.net/yugolf/ss-243892298" title="Reactive systems that focus on availability" target="_blank">Reactive systems that focus on availability</a> </strong> </div>


<iframe src="https://speakerdeck.com/player/0b8606f26e2448719c33257ad2f9f6a2" width="510" height="420" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen> </iframe>
<div style="margin-bottom:5px"> <strong> <a href="https://speakerdeck.com/player/0b8606f26e2448719c33257ad2f9f6a2" title="Challenged to reduce stateful application downtime to less than 10 seconds" target="_blank">Challenged to reduce stateful application downtime to less than 10 seconds</a></strong> </div>

## License
This content is compliant with  [Apache License 2.0](https://fintan.jp/?page_id=5803&lang=en).

 \* The names of the companies and products described in this site are trademarks or registered trademarks of the respective companies.  
 \* Amazon Web Services, AWS are trademarks of Amazon.com, Inc. or its affiliates in the United States and/or other countries.  
 \* Akka is a trademark of Lightbend, Inc.

<a href="https://www.reactivemanifesto.org/"> <img style="border: 0; position: fixed; right: 0; top:0; z-index: 9000" src="//d379ifj7s9wntv.cloudfront.net/reactivemanifesto/images/ribbons/we-are-reactive-blue-right.png"> </a>


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