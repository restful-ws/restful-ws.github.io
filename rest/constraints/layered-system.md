---
layout: default
title: Layered System Contraint
permalink: /rest/constraints/layered-system
---
## The Layered System Constraint

Source
: Fielding Dissertation, [Section 5.1.6](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm#sec_5_1_6)

### The Constraint

The system may be composed of hierarchical layers; 
no layer may have knowledge about the system beyond
the layer itself.

The layered system constraint introduces the concept
of intermediaries: gateways and proxies.

#### Defining Layered System

According to Fielding ([link](https://www.ics.uci.edu/~fielding/pubs/dissertation/net_arch_styles.htm#sec_3_4_3)):
> ...the layered system style allows an architecture 
> to be composed of hierarchical layers by 
> constraining component behavior such that each 
> component cannot "see" beyond the immediate layer 
> with which they are interacting. By restricting 
> knowledge of the system to a single layer, we place 
> a bound on the overall system complexity and 
> promote substrate independence.
> 
> Layers can be used to encapsulate legacy services 
> and to protect new services from legacy clients, 
> simplifying components by moving infrequently used 
> functionality to a shared intermediary. Intermediaries 
> can also be used to improve system scalability by 
> enabling load balancing of services across multiple 
> networks and processors.

### Rationale

Layered System provides much of what is required
for the Web to operated at Internet-scale.  It
introduces intermediaries while preventing
the kind of complexity that might occur if
separate layers of the system are designed
together. Layered System also accounts for 
the tremendous flexibility
found in modern Web infrastructure.

Layered System comes at a cost; as
Fielding identified, those
layers require overhead and increase
latency.

### Implications of Uniform Interface

XYZ
: TBD