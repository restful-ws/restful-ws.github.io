---
layout: default
title: The Representations Contraint
permalink: /rest/constraints/representations
---

## Manipulation of Resources through Representations

Source
: Fielding Dissertation, [Section 5.2.1.2](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm#sec_5_2_1_2)

### The Constraint

Resources are interacted with and manipulated by passing representations of the resource's current or intended state.

#### Defining Manipulation of Resources through Representations

A representation is a digital sequence of bytes that
expresses a resource's state, including any
metadata needed to correctly interpret it.

According to Fielding:
> REST components perform actions on a resource by 
> using a representation...

Regarding resources:
> A representation consists of data, metadata describing 
> the data, and, on occasion, metadata to describe the 
> metadata (usually for the purpose of verifying message 
> integrity). Metadata is in the form of name-value pairs, 
> where the name corresponds to a standard that defines 
> the value's structure and semantics. Response messages 
> may include both representation metadata and resource 
> metadata: information about the resource that is not 
> specific to the supplied representation.



### Rationale

The resources being represented are quite freqently
non-digital things.  They can be _anything_, and
they often do not fit in a wire, through an optical 
or on a disk somewhere.  Thus, we work with digital
representations of them to provide ourselves
something with which to interact.

In REST, payloads are representations of the state
of the identified resources.  What counts for a
representation is up to the author; REST imposes
no constraint on the representation's format, nor
its content.  However, there is an expectation
that the identified thing is a resource, it has
semantics, and that a representation reflects
its state.

In REST, the meaning of a message 
is a function of the semantics provided as the
message-bearing protocol's interaction semantics and metadata,
the semantics of the resource, and the semantics
of the representation format.

## Observing Manipulation of Resources through Representations in the Modern Web

TBD

## Implications of Manipulation of Resources through Representations

Messaging Protocol Must Provide Interaction Methods 
: asdf

The requirement for client competency
: TBD

Discarding resource-orientation does harm
: TBD

## How to Mess It Up