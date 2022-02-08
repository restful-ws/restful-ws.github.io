---
layout: default
title: Understanding REST
permalink: /rest/understanding-rest
---

# Understanding REST

The World Wide Web was among the most important 
inventions of the twentieth century.  It owes
much of its success to REST, the architecture
style that makes it work so well.  Decades after
REST and the Web were introduced, their
importance in business, civil society 
and the global economy continue to grow.

Despite its ubiquity and influence, REST remains
broadly misunderstood. As a renaissance of
integrated solutions transforms the delivery of
day-to-day services, the Web and REST provide
the platform. The designers of Web-based
solutions, in particular those claiming to
provide "REST APIs", often unknowingly
misrepresent their work product.  They
produce work that may better be described
as Resource-Oriented Service Integration, 
or ROSI.

Despite widespread 
[misappropriation of the term](https://twobithistory.org/2020/06/28/rest.html), 
REST, when understood as 
its originator conceived,
provides something quite special.  
API authors who fully embrace 
Fielding's REST achieve benefits 
beyond what 
resource-oriented Web API
authors enjoy.

For an API or Web Service
author aiming
to produce faithfully REST-based
solutions, this primer provides 
comprehensive, nuanced coverage of
REST to enable their work to
reach the potential of the modern
Web.

### REST: Origins

REST is the underlying architecture style
of the World Wide Web.  It stands for
_Representational State Transfer_, a
term that captures how REST centers
on the transfer of
_digital representations_ of resource
states as its core activity.

REST was invented in the mid-1990s 
by Roy Fielding, who unveiled REST
in his 2000 doctoral dissertation. HTTP, 
HyperText Transfer Protocol, is the
primary protocol of the World Wide 
Web. Fielding, one of HTTP's primary authors,
developed REST
as a collection of constraints that
could explain and justify design
choices made in its formal specification.
REST's constraints
bring to life the Web's most important
features and advantages.

### REST vs the Web

Despite a strong association, REST and
the World Wide Web are not the same.
REST is an architecture style, a set
of constraints that, when applied to
a solution, produce the characteristics
sought for the World Wide Web.  The
World Wide Web is the network
of interconnected resources and 
associated technologies; it is
pervasive, yet concrete, and 
provides the familiar content 
and services we find through our
browsers and Web API-enabled
apps.  REST is the style,
the Web is REST's premier 
implementation.

REST's constraints could be applied
to an entirely separate solution.
While that solution may have familiar
elements -- resources, identifiers,
formal content type descriptors,
and a client-server interaction
pattern -- the solution could also
use different formats, protocols,
and patterns.  The World Wide
Web is a REST-based solution, but
not all REST-based solutions are
the Web.

### What Was REST Aiming For?

In drafting the HTTP standard, Fielding 
and the HTTP specification drafting team 
had the Web's key features in mind.  
Meanwhile, the same team was involved
in a much larger conversation about the
nature of the web, best captured by
Tim Berners-Lee in the 
[W3C's Design Issues Pages](https://www.w3.org/DesignIssues/).

What were the Web's key features?

A Browsable Web of Linked Documents
: A user would use the Web through a *browser*
that could consume present the Web's documents.
The documents would contain links, enabling
the user to direct the browser to other 
documents and interact with the Web's features.

Anarchically Managed Systems and Content
: Content can be contributed by anyone.
Resources could be linked by any author.  The
systems providing the content are
managed independently, with no requirement
for coordination.

Durability, Reliability
: The failure of an individual system would not
impact the reliability of the Web.  The
underlying mechanics of the Web enable and
promote resilience of the independent systems
and of any individual resource.  

Multimedia, A Diversity of Content Types
: Though a number of primary content types
were favored, the web could support any
type of content that a browser could
understand.  Readable documents, video,
still images, audio, interactive content,
structured content, and anything that
could be conveyed in digital form
was in focus.

Low Technical Requirement For Access
: Despite the flexibility, the minimum
requirements for accessing the Web
are low; the client must understand
HTTP semantics, the media formats it
expects to encounter, have the 
network access needed, and be
able to support interactions with
its user or consumer.

Independently Evolving Components
: The Web's components and content
evolve independently.  Changes can
occur without imposing technical 
changes to other components. New 
content may be published without 
requiring browser changes.

> TDB: Need to review this list against
> Fielding, W3C:Web Architecture, and
> W3C:Design Issues.
>
> Crucial elements may be missing,
> such as the web's universal
> namespace for resources.

### REST's Constraints in Brief

Fielding's dissertation provided ten
constraints for REST.  Six are 
_**primary**_ constraints:
- Client-Server
- Stateless
- Caching
- Uniform Interface
- Layered System
- Code On Demand

Four additional constraints inform the 
**_Uniform Interface_** constraint:
- Resource Identification
- Manipulation of Resources through Representation
- Self-describing Messages
- Hypermedia (as the Engine of Application State)

The ten constraints ensure that web clients and
web services have appropriate separation of concerns,
convey the information necessary for each component
to perform its tasks, avoid compromising state issues,
and provide sufficiently informative messaging to
make the interconnected web possible.

### Implications for REST solutions

> **Loose Coupling** as a pattern that emerges from
> multiple constraints.  Client-server, stateless,
> layered system, uniform interface

> **Client Competency** as a requirement that emerges
> from Stateless and Self-descriptive Messages

> **


### Realizing REST in the Modern Web 

REST's constraints had a broad range of impacts.

**Syntax**: REST requires a messaging protocol
that can express messages (TBD)

**Semantics**: REST requires a messaging protocol
that can express messages (TBD)

- HTTP Semantics
- Representation Semantics
- Resource Semantics

**Solution**: REST requires a messaging protocol
that can express messages (TBD)

### The Requirement for Client Competency






### REST for APIs: Often Misunderstood

abc

### REST vs ROSI 

abc