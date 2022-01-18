---
layout: default
title: Understanding REST
permalink: /rest/understanding-rest
---

## Understanding REST

The World Wide Web was among the most important 
inventions of the twentieth century.  It owes
much of its success to REST, the architecture
style that makes it work so well.  Decades after
the REST and the Web were introduced, their
importance in business, civil society, and
the economy continue to grow.

Despite its ubiquity and influence, REST remains
broadly misunderstood. As a renaissance of
integrated solutions transforms the delivery of
day-to-day services, the Web and REST provide
the platform. The designers of Web-based
solutions, in particular those claiming to
provide "REST APIs", often unkowningly
misrepresent their work product.  They
produce work that may better be described
as Resource-Oriented Service Integration, 
or ROSI.

Despite the misappropriation of the term, 
REST, as its creator originally conceived,
provided something special.  Moreover,
API authors who embrace REST as it
was originally conceived may see tremendous
opportunity in faithfully applying REST 
to their work.

For a REST Web Service designer aiming
to produce faithfully REST-informed
solutions this primer provides 
comprehensive, nuanced coverage of
REST and the technologies that make
the modern Web

### REST: Origins

REST is the underlying architecture style
of the World Wide Web.  It stands for
_REpresentational State Transfer_, a
term that captures how REST centers
on the transfer of
_digital representations_ of resource
states as its core activity.

REST was invented in the mid-1990s 
by Roy Fielding, who unveiled REST
in his doctoral dissertation in 2000.
Fielding, a primary author of the HTTP
protocol specification.  HTTP, 
HyperText Transfer Protocol, is the
primary protocol of the World Wide 
Web. Fielding developed REST
as a framework of constraints that
could explain and justify design
choices made in HTTP's specification,
constrains that would enable HTTP to
bring to life the Web's most important
features and advantages.

### REST vs the Web

Despite a strong association, REST and
the World Wide Web are not the same.
REST is an architecture style, a set
of constraints that, when applied to
a solution, produce the characteristics
sought for the World Wide Web.  The
World Wide Web itself is the network
of interconnected resources and 
associated technologies, something
pervasive, yet concrete, that 
provides the Web's familiar content 
and services.

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

A Browseable Web of Linked Documents
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

Independently Evolvable
: The Web's components and content
evolve independently.  Changes can
occur without imposing technical 
changes to other components. New 
content may be published without 
requiring browser changes.

TBD: This non-breaking thing is
a big deal!  

### REST's Constraints in Brief

Fielding's dissertation provided ten
constraints for REST.  Six are 
_primary_ constraints:
- Client-Server
- Stateless
- Caching
- Uniform Interface
- Layered System
- Code On Demand

Four additional constraints inform the 
Uniform Interface constraint:
- Resource Idenetification
- Manipulation of Resources through Representation
- Self-describing Messages
- Hypermedia (as the Engine of Application State)

In this primer, the constraints will be described
in depth.  





##### TBD - Informing Syntax, Semantics





### REST for APIs: Often Misunderstood

### REST vs ROSI 

