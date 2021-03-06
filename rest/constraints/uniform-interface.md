---
layout: default
title: Uniform Interface Contraint
permalink: /rest/constraints/uniform-interface
---

## The _Uniform Interface_ Constraint

Source
: Fielding Dissertation, [Section 5.1.5](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm#sec_5_1_5)

### The Constraint

Regardless of service or resource offered or rendered, 
the interface will be generic.

This constraint relies on four additional constraints, 
which play an integral role in defining services and
resources:
- [Resource Identification](/rest/constraints/resource-identification): REST interactions are always in the context of an identified resource.
- [Manipulation of Resources through Representation](/rest/constraints/representations): Resources are interacted with and manipulated by passing representations of the resource's current or intended state.
- [Self-describing Messages](/rest/constraints/self-descriptive-messages): Each message must contain the information needed to understand the request.
- [Hypermedia as the Engine of Application State](/rest/constraints/hypermedia): The application's state is driven through transitions that occur through hypermedia links.

#### Defining Uniform Interface

According to Fielding ([link](https://www.ics.uci.edu/~fielding/pubs/dissertation/net_arch_styles.htm#sec_3_4_3)):
> The central feature that distinguishes the REST 
> architectural style from other network-based styles 
> is its emphasis on a uniform interface between components... 
> By applying the software engineering 
> principle of generality to the component interface, 
> the overall system architecture is simplified and 
> the visibility of interactions is improved. 
> Implementations are decoupled from the services they 
> provide, which encourages independent evolvability.

### Rationale

A client implemented against a specific interface may
be said to be _tightly coupled_ with it. This leads
to the need to change the client whenever the interface
changes.  If the client must integrate with another
service, that integration will take more work, since
it, too, must be implemented.  If the client has not
yet implemented the interface for a service, it cannot
use it.

The Web would not function if the browser needed to
have updates whenever a new service was offered.  
As an anarchically managed network, the web must
present an interface that applies to any resource
or service. 

_Uniform Interface_ simplifies the Web architecture by
requiring generic interfaces.  Instead of adapting the
client to the network, the client must merely
know the semantics of the protocols and media types
for which it is intended.  Separating the Web's
components this way enables independent evolvability.

Fielding pointed out a crucial negative tradeoff 
of Uniform Interface; efficiency is reduced due 
to the generalized interface.

## Observing _Uniform Interface_ on the Modern Web

> TBD: HTTP Semantics
>> HTTP Methods
>
>> HTTP Status Codes
>
>> HTTP Headers

> IANA Registries 
>> Media Types
> 
>> Link Relations
> 
>> And so on


## Implications of Uniform Interface

> Client Competency

> Design Implication:  What About My Interface Semantics?


## How to Mess It Up

- Invent your own HTTP Methods

- Ignore protocol method semantics

- Use POST for Everything

- Interpret HTTP Semantics as CRUD

