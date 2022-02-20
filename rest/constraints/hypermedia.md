---
layout: default
title: Hypermedia Contraint
permalink: /rest/constraints/hypermedia
---

## The _Hypermedia as the Engine of Application State_ Constraint

Source
: Fielding Dissertation, [Section 5.3.1](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm#sec_5_3_1)

### The Constraint

A REST application's state is driven through transitions that occur through hypermedia links.

#### Defining Hypermedia as the Engine of Application State


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

## Observing Hypermedia in the Modern Web


### Implications of Hypermedia

The requirement for client competency
: TBD


## How to Mess It Up