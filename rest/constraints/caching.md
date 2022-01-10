---
layout: default
title: Caching Contraint
permalink: /rest/constraints/caching.html
---

## The Caching Constraint

Source
: Fielding Dissertation, [Section 5.1.4](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm#sec_5_1_4)

### The Constraint

Content cacheablity in responses must be implicitly or 
explicitly indicated.  Clients (and intermediaries) have
the right to use cached content in lieu of make
equivalent requests later.

#### Defining Caching

According to Fielding ([link](https://www.ics.uci.edu/~fielding/pubs/dissertation/net_arch_styles.htm#sec_3_4_3)):
> A cache acts as a mediator between client and server 
> in which the responses to prior requests can, if they 
> are considered cacheable, be reused in response to 
> later requests that are equivalent and likely to result 
> in a response identical to that in the cache if the 
> request were to be forwarded to the server.

### Rationale

Cache improves efficiency and perceived application latency
by eliminating the need for some transactions.  It also
improves scalability by reducing the use of network and
compute resources.

Fielding pointed out negative tradeoffs of caching; 
when stale cached content
is used, the user experience 
can suffer due to its reliance on outdated information.

### Implications of Caching

Cacheability must be Planned 
: TBD

Cacheability requires Resource State
: TBD.  The ability to indicate that content
may be cached requires that the resource
itself must be understood as having state.  The
caching requirement cannot be met if the 
target of the request is transient or stateless,
such as an RPC interface or a database-like
query interface.

