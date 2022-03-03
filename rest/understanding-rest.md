`---
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
the platform. The designers of web services,
in particular those claiming to
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

## Origins

REST is the underlying architecture style
of the World Wide Web.  It stands for
_Representational State Transfer_, a
term that captures how REST centers
on the transfer of
_digital representations_ of resource
states as its core activity.

REST was conceived in the mid-1990s 
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

## REST vs the Web

Despite a strong association, REST and
the World Wide Web are not the same.
REST is an architecture style, a set
of constraints that, when applied to
a system, produces the characteristics
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

## What Was REST Aiming For?

In drafting the HTTP standard, Fielding 
and the HTTP specification drafting team 
had the Web's key features in mind.  
Meanwhile, the same team was involved
in a much larger conversation about the
nature of the web, best captured by
Tim Berners-Lee in the 
[W3C's Design Issues Pages](https://www.w3.org/DesignIssues/).

What were the Web's key features?

A Browsable Web of Linked Resources
: A user would use the Web through a *browser*
that could consume present the Web's 
resources, usually documents.
The representations, often HTML, 
would contain links, enabling
the user to direct the browser to other 
resources and interact with the Web's features.

Anarchically Managed Systems and Content
: Content can be contributed by anyone.
Resources could be linked by any author.  The
systems providing the content are
managed independently, with no requirement
for coordination.

Durability, Reliability
: The failure of an individual system should
not impact the reliability of the Web.  The
underlying mechanics of the Web should
promote resilience of the independent systems
and of any individual resource.  

Multimedia, A Diversity of Content Types
: The web should support any
type of content that a browser or client
can understand.  Readable documents, video,
still images, audio, interactive content,
structured content, and anything that
could be conveyed in digital form
was in focus.

Low Technical Requirement For Access
: Despite the flexibility, the minimum
requirements for accessing the Web
should be low; 
the client must understand
HTTP semantics, the media formats it
expects to encounter, have the 
network access needed, and be
able to support interactions with
its user or consumer.

Independently Evolving Components
: The Web's components and content
evolve independently.  Changes can
occur without imposing technical 
changes to other components. 
For example, newly published content
should require browser changes.


> TDB: Need to review this list against
> Fielding, W3C:Web Architecture, and
> W3C:Design Issues.
>
> Crucial elements may be missing,
> such as the web's universal
> namespace for resources.

## REST's Constraints in Brief

Fielding's dissertation provided REST's ten
constraints.   

Six are _**primary**_ constraints:
- [Client-Server](/rest/constraints/client-server): REST interactions are between _client_ and _server_.  Supports _separation of concerns_.
- [Stateless](/rest/constraints/stateless): Session state is _never_ stored with the server.
- [Caching](/rest/constraints/caching): Components may cache responses when the cacheability is indicated.
- [Uniform Interface](/rest/constraints/uniform-interface): Regardless of service or resource, its interface will be generic.
- [Layered System](/rest/constraints/layered-system): No component or layer may have knowledge of the system beyond the layer itself.
- [Code On Demand](/rest/constraints/code-on-demand): The server may facilitate client processing by providing code to the client.

Four additional constraints inform the 
**_Uniform Interface_** constraint:
- [Resource Identification](/rest/constraints/resource-identification): REST interactions are always in the context of an identified resource.
- [Manipulation of Resources through Representation](/rest/constraints/representations): Resources are interacted with and manipulated by passing representations of the resource's current or intended state. 
- [Self-describing Messages](/rest/constraints/self-descriptive-messages): Each message must contain the information needed to understand the request.
- [Hypermedia as the Engine of Application State](/rest/constraints/hypermedia): The application's state is driven through transitions that occur through hypermedia links.  

The ten constraints ensure that web clients and
web services have appropriate separation of concerns,
convey the information necessary for each component
to perform its tasks, avoid compromising state issues,
and provide sufficiently informative messaging to
make the interconnected web possible.

## Implications for REST solutions

> **Loose Coupling** as a pattern that emerges from
> multiple constraints.  Client-server, stateless,
> layered system, uniform interface

> **Client Competency** as a requirement that emerges
> from Stateless and Self-descriptive Messages

Semantic Observability, Managability
: For sufficiently competent observer,
REST messages contain everything needed
to understand the message's meaning.
No out-of-band information needed and
no privileged state-related information
must be known to interpret the message.
In addition to providing beneficial
architectural advantages, 
Semantic Observability means that a
solution's communication can be managed.
**TBD** Externalized management of
semantics is a game changer; monolithic
architectures and solutions with
privileged meaning embedded in messaging
are harder to manage by businesses.
With organizations pursuing API-led
digital transformation, REST provides
an ideal foundation for expressing
their resources and capabilities.


## Realizing REST in the Modern Web 

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

### The Client Competency Requirement

_Client Competency_, which may also be
referred to as _component_ or _observer_
_competency_, are the capabilities needed
to understand the REST messages pertaining
to the component's function.

For the modern web, any client must 
understand HTTP message construction.
The client must understand HTTP semantics,
the request methods, response codes, the
use of URIs, and the request and response
headers it will encounter.

Crucially, the client must understand the
media types it will encounter.  A typical
web browser will understand HTML, CSS,
Javascript, web fonts, image formats, 
and audio/video formats.  Other types
of web clients may support a completely
different set of formats, but will have
HTTP protocol semantics in common.

Beyond having a single URI as
a starting point, a REST client may
**not** be designed with knowledge of
the URI surface of a server or service.
Despite it being common for
URI and URI-associated schema sharing
to enable HTTP API clients
to interact with services, the
practice results in a non-REST system.
This is due to the system violating the 
_Self-Describing Messages_ constraint, 
the reliance on privileged out-of-message
information to drive application state.

## Manageable Semantics: The Externalization of System Semantics

Since REST makes a system's communication
observable and externally undestandable.
This exposure of a system's semantics
gives rise to the opportunity to manage
the meaning conveyed in the system. 
Alongside the resource-oriented nature 
of REST communication, the architecture
style is a good fit for enabling realization of
entity-modeled systems.

TBD: Go further to suggest that whole-enterprise
transformation through domain-driven reduction and
REST-based realization is a good idea?


### REST for APIs: Often Misunderstood

abc
`
### REST vs ROSI 

abc