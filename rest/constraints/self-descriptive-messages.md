---
layout: default
title: Self-descriptive Messages Contraint
permalink: /rest/constraints/self-descriptive-messages
---

## The Self-descriptive Messages Constraint

Source
: Fielding Dissertation, [Section 5.3.1](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm#sec_5_3_1)

### The Constraint

Each message must contain the information needed to understand the request.

#### Defining Self-descriptive Messages

According to Fielding:
> REST enables intermediate processing by constraining
> messages to be self-descriptive: interaction is 
> stateless between requests, standard methods and media
> types are used to indicate semantics and exchange 
> information, and responses explicitly indicate cacheability.


### Rationale

Message self-description provides a number of
benefits.
- Improved Reliability:  Any component instance
can understand and serve the request, so 
failing components can be removed without risk
to application state.
- Observability: Intermediaries and observing
components can fully understand communication.

Statelessness is required to achieve message
self-description; if information known elsewhere
is required to correctly interpret the message,
the message itself cannot sufficiently describe
itself.

Having _standard_ methods and media
types enables message-processing components to
implement the semantics and formats prior to
encountering them in messages.  Thus,
self-description relies on a level of
_fluency_ or _competency_ in the message
processor.

### Examples
- A
- B

### Implications of Resource Identification

The requirement for client competency
: TBD
