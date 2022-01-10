---
layout: default
title: Resource Identification Contraint
permalink: /rest/constraints/resource-identification.html
---

## The Resource Identification Constraint

Source
: Fielding Dissertation, [Section 5.2.1.1](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm#sec_5_2_1_1)

### The Constraint

REST interactions are always in the context of an identified resource.

#### Defining Resource and Resource Identification

According to Fielding:
> The key abstraction of information in REST is a resource.

Regarding resources:
> Any information that can be named can be a resource: a 
> document or image, a temporal service (e.g. "today's weather 
> in Los Angeles"), a collection of other resources, a 
> non-virtual object (e.g. a person), and so on. In other 
> words, any concept that might be the target of an author's 
> hypertext reference must fit within the definition of a 
> resource. A resource is a conceptual mapping to a set of 
> entities, not the entity that corresponds to the 
> mapping at any particular point in time.

Regarding resource identifiers:
> REST uses a resource identifier to identify the particular 
> resource involved in an interaction between components. 
> REST connectors provide a generic interface for accessing and 
> manipulating the value set of a resource...

Finally:
> ...the only thing that is required to be static for a 
> resource is the semantics of the mapping, since the 
> semantics is what distinguishes one resource from another.


### Rationale

Resources
: Using resources as the context of REST interactions is called
_resource orientation_.  Resource orientation enables the
generalized interface (_Uniform Interface_) to rely on
the semantics of the resource, whatever it is.  This
choice provides enourmous flexibility to the authors
of the Web's resources and services.

Resource Identifiers
: In relying on resource-centric semantics for REST messages,
the resources themselves must, naturally, be identified.
Using resource identifiers in messages provides for
decentralization of the services offered, avoids
problems to scale that centralization imposes, and
enables a system to cross organization and 
domain boundaries.


### Examples
- A
- B

### Implications of Resource Identification

XYZ
: TBD