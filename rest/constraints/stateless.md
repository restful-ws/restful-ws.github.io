---
layout: default
title: Client-Server Contraint
permalink: /rest/constraints/stateless
---

# The _Stateless_ Constraint

Source
: Fielding Dissertation, [Section 5.1.3](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm#sec_5_1_3)

## The Constraint

Session state is _never_ stored with the server.

In other words, the server must not store information needed to understand the
client's request.

### Defining Stateless
According to Fielding ([link](https://www.ics.uci.edu/~fielding/pubs/dissertation/net_arch_styles.htm#sec_3_4_3)):
> The client-stateless-server style derives from client-server 
> with the additional constraint that no session state is 
> allowed on the server component. Each request from client to 
> server must contain all of the information necessary to 
> understand the request, and cannot take advantage of any 
> stored context on the server. Session state is kept entirely 
> on the client.

## Rationale

_Stateless_ requires that a system, *by design*, avoids
server-side management of client state.  Strengthening
[client-server](/rest/constraints/client-server) 
separation and 
[Self-descriptive Messages](/rest/constraints/self-descriptive-messages),
the constraint 
doubles down on avoidance of client-server
intermingling, both in design and in use.

A number of architectural anti-patterns can be seen
when client and server are intermingled.
1. Server-managed client state introduces
a failure point that need not exist.
2. Server management of client state requires
data persistence and processing which, at scale,
can impede server performance.
3. Management of client state ensures that
the meaning of a request cannot be understood
through the message alone, undermining the
[Self-Descriptive Messages]() constraint and
its benefits.

In Fielding's words, the _Stateless_ constraint provides 
visibility, reliability, and scalability.

> Visibility is improved because a monitoring system does 
> not have to look beyond a single request datum in order 
> to determine the full nature of the request. Reliability 
> is improved because it eases the task of recovering from 
> partial failures [133]. Scalability is improved because 
> not having to store state between requests allows the 
> server component to quickly free resources, and further 
> simplifies implementation because the server doesn't have 
> to manage resource usage across requests.

Fielding also points out negatives in the trade-off; the
constraint decreases network performance by increasing
repetitive data exchange and diminishes the server's
control over application behavior.

## Observing Stateless in the Modern Web

> TBD:  Need a discussion of how, when implemented well,
> stateless improve scale, visibility, and durability.
> Needs a picture.

> TBD: Discussion of *Cookies* and how this violates
> client state.  Session cookies.  Authorization
> cookies.  Encrypted content within tokens.

> TBD: Brief coverage of authorization patterns and
> how they relate to REST.  OAuth2.  Opaque vs
> Structured (JWT) auth tokens

## Implications of Stateless

Together, the _Client-Server_, _Stateless_, and
resource-oriented constraints that 
support _Uniform Interface_ lead to the
separation of application state from resource 
state. 

**Client** is responsible for **application state**.
**Server** is responsible for **resource state**.

The clean separation of application and resource state,
a part of separating of client and server concerns, 
are part of what makes REST solutions scalable and
evolvable.

TBD: What about other components?
: TBD

## How to Mess It Up

To undermine client-server separation:
1. Design the client and server together.
2. Manage application state on the server. This includes producing
cookies for the client to store that only the server understands.
3. Build intermediaries that understand and manipulate messages
according to privileged information about the client, server, or resource.









