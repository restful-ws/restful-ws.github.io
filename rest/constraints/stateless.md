---
layout: default
title: Client-Server Contraint
permalink: /rest/constraints/stateless
---

# The _Stateless_ Constraint

Source
: Fielding Dissertation, [Section 5.1.3](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm#sec_5_1_3)

## The Constraint

Session state is _never_ stored with the server.  Each request must contain the
information needed to understand the request.

In other words, the server may not store information needed to understand the
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
[client-server]() separation, the constraint 
doubles down on avoidance of client-server
intermingling, both in design and in the
application session.

A number of architectural anti-patterns can be seen
when client and server are intermingled.
1. Server-managed client state introduces
a point of failure that should not exist.
2. Server management of client state requires
data persistence and processing which, at scale,
can prevent the solution from performing.
3. Management of client state ensures that
the meaning of a request cannot be understood
through the message alone, undermining the
[Self-Descriptive Messages]() constraint and
its benefits.

In Fielding's [describes]() words, the _    _ constraint provides 
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

Client State == Application state
: TBD

Server State == Resource State
: TBD

Client State vs Server State 
: TBD

TBD: What about other components?
: TBD

