---
layout: default
title: Resource Identification Contraint
permalink: /rest/constraints/resource-identification
---

## The Resource Identification Constraint

Source
: Fielding Dissertation, [Section 5.2.1.1](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm#sec_5_2_1_1)

### The Constraint

REST interactions are always in the context of an identified resource.

#### Defining Resource Identification

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



> TBD: The W3C's view on URI opacity. 


### Rationale

REST interactions need context.  If interactions are 
constrained to using a generic, _Uniform Interface_
for interactions, to what are these interactions
directed?  What do the requests mean?  The 
_Resource Identification_ constraint provides this
context.

REST was developed as the object-oriented design 
was gaining traction.  In 
*Object Oriented Programming* (OOP),
procedural logic is associated with objects.
Procedural functions and variables, when associated
with objects, became the object's methods and
attributes, respectively.  Fielding's REST
promoted the early Web's _documents_ into 
_resources_, full-fledged, semantically-informed
interactable entities.

REST interactions are always with identified _resources_; on
the modern Web, we use URIs to identify them.

Resources
: Using a resource as the context of a REST interaction is 
called
_resource orientation_.  Resource orientation enables the
generalized interface (_Uniform Interface_) to rely on
the _semantics of the resource_, whatever that resource
is.  Resource orientation
provides enormous flexibility to the authors
of the Web's resources and services, while maintaining 
the
need for the resource to express itself through the
generic interface.

Resource Identifiers
: Relying on resource-centric semantics, REST messages
must identify the resource that provides the
context.
Using resource identifiers in messages provides for
decentralization of the services offered, avoids
problems to scale that centralization imposes, and
enables a system to cross organization and 
domain boundaries.

## Observing _Resource Identification_ on the Modern Web

Of all the constraints, _Resource Identification_ may
be the easiest to spot in the wild.

## Implications of Resource Identification

XYZ
: TBD

## How to Mess It Up