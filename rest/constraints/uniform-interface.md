---
layout: default
title: Uniform Interface Contraint
permalink: /rest/constraints/uniform-interface.html
---

## The Uniform Interface Constraint

Source
: Fielding Dissertation, [Section 5.1.5](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm#sec_5_1_5)

### The Constraint

Regardless of service or resource offered or rendered, 
the interface will be generic.

This constraint relies on four additional constraints, 
which play an integral role in defining services and
resources:
- [Resource Identification]()
- [Representations]()
- [Self-descriptive Messages]()
- [Hypermedia]()

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

Uniform Interface simplifies the system's architecture
and separates the implementations of components from the
services, enabling greater independence among components.

Fielding pointed out negative tradeoffs of Uniform Interface;
efficiency is reduced due to the generalized interface.

### Implications of Uniform Interface

XYZ
: TBD
