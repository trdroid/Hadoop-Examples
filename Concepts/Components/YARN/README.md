# YARN

YARN (Yet Another Resource Negotiation) is Hadoop's distributed resource scheduler. It was primarily created to schedule, manage and monitor resources in a Hadoop cluster. 

YARN is made of

* YARN Framwork, a framework that handles resource scheduling, managing and monitoring
* YARN applications that are executed in a cluster

### YARN Framework

The YARN frameworks offers the following functionality

1. **Resource scheduling**
    
  The resources that YARN framework schedules are *containers*. The requests for the allocation of the *container* resources come from the YARN applications. The YARN framework evalutes these requests and attempts to allocate *containers* to the requested YARN applications.

2. **Resource Monitoring**

  The YARN framwork monitors the allocated *containers* to
  
  * reuse the freed-up resources to schedule additional work
  * terminate rogue containers that fail to abide by their contract

**YARN Framework: Features**

The YARN framework has the following features that make it scale better than MapReduce

* Stateless
  
  The YARN framwork does not hold the state of the applications that are executed on the cluster.

* Application-agnostic

  The YARN framework is desgined to run any application on the cluster without caring out what type of application it is.
  
**YARN Framework: Core Components**

* ResourceManager
* NodeManager

**YARN Applications: Core Components**

* YARN Application client
* ApplicationMaster
* Container

**Why YARN was introduced?**

YARN was introduced in Hadoop version 2 in response to the following limitations in Hadoop version 1.

1. **Limited Workload Support**:
2. **Scalability Issues**:
3. **Underutilization of resources**:
