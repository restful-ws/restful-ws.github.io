---
layout: default
title: Client-Server Constraint
permalink: /rest/constraints/client-server
---

## The _Client-Server_ Constraint

Source
: Fielding Dissertation, [Section 5.1.2](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm#sec_5_1_2)

## The Constraint

All REST interactions are between _client_ and _server_.

### Defining Client and Server
According to Fielding ([link](https://www.ics.uci.edu/~fielding/pubs/dissertation/net_arch_styles.htm#sec_3_4_1)):
> A **server** component, offering a set of services, 
> listens for requests upon those services. A **client** component, 
> desiring that a service be performed, sends a request to the 
> server via a connector. The **server** either rejects or performs the 
> request and sends a response back to the client.
> <br/> -- Fielding  

### Rationale

The Client-Server constraint enables _Separation of Concerns_.  

Client-server requires that the two entities be distinct 
components that communicate with one another with messages.
In addition, the nature of that communication is such
that the client initiates communication and the server 
responds; a _peer-to-peer_ communication style, for
example, does not meet the requirement.

The Client-Server constraint provides part of the
basis for _loose coupling_ among components. 
Loosely coupled components are not designed
specifically to integrate with one another; they
meet a more generic set of requirements that
enables interoperability regardless of the
other component's specifics.

Benefits of Client-Server:
- improves _scalability_
- simplifies both client and server
- enables client and server to evolve independently

Per Fielding:
> **Separation of concerns** is the principle behind the client-server
> constraints. A proper separation of functionality should simplify
> the server component in order to improve scalability. This
> simplification usually takes the form of moving all of the user
> interface functionality into the client component. The separation
> also allows the two types of components to evolve independently,
> provided that the interface doesn't change.

## Observing Client-Server in the Modern Web

> TBD: Client-server relationship built into HTTP

```
Good Opportunity for a code block to illustrate that
in HTTP, 
```

> TBD: When they encounter unexpected content, browsers do not break.
> They merely do not support the unknown elements. They
> will ignore it or indicate non-support.

> `restful.ws` describes this feature as _client competency_


## Implications of Client-Server

Design-time Separation Of Concerns
: To achieve independent evolveability, Client and Server concerns must 
be separated at both runtime and design time.

Runtime Separation Of Concerns
: TBD

User Interface Concerns Abstracted from the Server
: TBD

## How to Mess It Up

## Diagrams

> TBD: Client-server vs Peer-to-peer?
> Is it useful to depict this?
> 