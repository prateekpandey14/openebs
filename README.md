# OpenEBS

[![Build Status](https://travis-ci.org/openebs/jiva.svg?branch=master)](https://travis-ci.org/openebs/jiva)
[![Docker Pulls](https://img.shields.io/docker/pulls/openebs/jiva.svg)](https://hub.docker.com/r/openebs/jiva/)
[![Slack](https://img.shields.io/badge/chat!!!-slack-ff1493.svg)]( https://openebsslacksignup.herokuapp.com/)
[![Slack](https://openebsslacksignup.herokuapp.com/badge.svg)]( https://openebsslacksignup.herokuapp.com/)
http://www.openebs.io/
 
OpenEBS enables the use of containers for mission critical, persistent workloads.  OpenEBS is containerized storage and related storage services.   
 
OpenEBS allows you to treat your persistent workload containers, such as DBs on containers, just like other containers.  OpenEBS itself is deployed as just another container on your host, and enables:storage services that can be designated on a per pod, application, cluster or container level, including:   
- Data persistence across nodes, dramatically reducing time spent rebuilding Cassandra rings for example
- Synchronization of data across availability zones and cloud providers
- Use of commodity hardware plus a container engine to deliver seriously scale out block storage
- Integration with orchestrators, so that developer and application intent flows into OpenEBS configurations automatically
- Management of tiering to and from S3 and other targets
- Plus we’re bringing our experience from BSD based containerization and delivering QoS for customers from our CloudByte experience over to OpenEBS - expect to see more intelligence and manageability 
 
Our vision is simple: let’s let storage and storage services for persistent workloads be so fully integrated into the environment and hence managed automatically that is almost disappears into the background as just yet another infrastructure service that works.  
 
## Why OpenEBS scales
 
OpenEBS can scale to include an  arbitrarily large number of containerized storage controllers  thanks in part to some advancements in the management of metadata which removes a common bottleneck to scale out storage performance.    Again, we learned the hard way over the years at CloudByte and are extremely happy to see initial scale out performance figures with OpenEBS; much credit goes to the orchestration and containerization of course as well.
 
## Installation and Getting Started
 
OpenEBS can be setup in few easy steps.  You can get going on GCE to try it out quickly here:  https://github.com/openebs/openebs/blob/master/k8s/hyperconverged/tutorial-configure-openebs-gke.md
Also, we have a Vagrant environment available that includes a sample Kubernetes deployment and synthetic load you can use to simulate the performance of OpenEBS. 
Please follow our [Getting Started](k8s/dedicated/README.md) documentation 
 
## Status
We are approaching beta stage with active development underway. See our [Project Tracker](https://github.com/openebs/openebs/wiki/Project-Tracker) for more details.
 
## Contributing
 
We welcome your feedback and contributions in any form possible.  
 
Please join us on Slack at:  https://openebs-community.slack.com/
 
- Join us at [openebs-slack-signup](https://openebsslacksignup.herokuapp.com/)
  - Already signed up ? Head to our discussions at [openebs-users channel](https://openebs-community.slack.com/messages/openebs-users/)
- Want to raise an issue ?
  - If it is a generic (or `not really sure`), you can still raise it at [issues](https://github.com/openebs/openebs/issues)
  - Project specific issues can be raised at individual project level.
- Want to help with fixes and features:
  - Have a look at [open issues](https://github.com/issues?q=user%3Aopenebs+is%3Aopen)
  - Have a look at [contributing guide](./CONTRIBUTING.md)

## Show me the Code

This is a meta-repository for OpenEBS. Here please find various documentation related artifacts and code related to integrating OpenEBS with popular orchestration engines like kubernetes, swarm, mesos, rancher, etc., The core storage and storage orchestration source code is distributed in other repositories under the OpenEBS organization. Please start with the pinned repositories or with [OpenEBS Architecture](./contribute/design/README.md) document. 

## License

OpenEBS is developed under Apache 2.0 License at the project level. 
Some components of the project are derived from other opensource projects like Nomad, Longhorn 
and are distributed under their respective licenses. 
