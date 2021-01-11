---
layout: post
title:  "Openshift Service Mesh"
date:   2020-09-10 12:21:00 -0500
categories: RedHat Openshift Kubernates
---

## Service Mesh ## 
is a network of microservices that make up applications and interactions between applications.<br> 
It can handle **Discovery, Load balancing, Failure recovery, Metrics and monitoring**. <br>
It can also provide complex operational requirements like **A/B testing, Canary releases, Rate limiting, Access control, End-to-end authentication**


## Istio ##
[Istio](www.istio.io) is a popular open source service mesh. An Istio service mesh is logically split into a data plane and a control plane.<br>
The data plane is composed of a set of intelligent [Envoy](https://www.envoyproxy.io/) proxies deployed as sidecars. <br>
Mixer is a control plane component which enforces access control and usage policies across the service mesh, and collects telemetry data from the Envoy proxy and other services. <br>
Pilot is another control plane componennt which provides service discovery for the Envoy sidecars, as well as traffic management capabilities for intelligent routing.<br>
Auth/Citadel is a control plane component which provides strong service-to-service and end-user authentication with built-in identity and credential management.<br>

 ## Installation ##
 1. Install Elasticsearch operator.
 2. Install Jeager operator.
 3. Install Kiali operator.
 4. Install Servicemesh operator.
 
 1. create project
 `oc adm new-project istio-system --display-name="Service Mesh System"`
 
 
 ## Resources ##
 [service mesh docs](https://docs.openshift.com/container-platform/4.5/service_mesh/v1x/installing-ossm.html)
 
