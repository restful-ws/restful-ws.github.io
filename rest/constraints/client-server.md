---
layout: default
title: Client-Server Contraint
permalink: /rest/constraints/client-server.html
---

## The Client-Server Constraint

Source
: Fielding Dissertation, [Section 5.1.2](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm#sec_5_1_2)

### The Constraint

All REST interactions are between _client_ and _server_.

#### Defining Client and Server
According to Fielding ([link](https://www.ics.uci.edu/~fielding/pubs/dissertation/net_arch_styles.htm#sec_3_4_1)):
> A **server** component, offering a set of services, 
> listens for requests upon those services. A **client** component, 
> desiring that a service be performed, sends a request to the 
> server via a connector. The **server** either rejects or performs the 
> request and sends a response back to the client.
> <br/> -- Fielding's dissertation, section  

### Rationale

The purpose of the Client-Server constraint is to enable _Separation of Concerns_.

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

### Implications of Client-Server

Design-time Separation Of Concerns
: To achieve independent evolvability, Client and Server concerns must 
be separated at both runtime and design time.

Runtime Separation Of Concerns
: TBD
