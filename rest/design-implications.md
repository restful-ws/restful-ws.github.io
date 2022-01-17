---
layout: default
title: Design Implications for APIs
permalink: /rest/constraints/design-implications.html
---

## Design Implications for Web APIs

Building upon Fielding's dissertation and formal REST,
the World Wide Web Consortium's
[_Architecture of the World Wide Web, Volume One_](https://www.w3.org/TR/webarch)
provides crucial foundations and clarifications that
inform good practice for Web API design.  In addition,
decades of work by the Internet Engineering Task Force
provides practical foundation that did not exist
at the time of Fielding's writing.  These include
numerous [RFCs](https://www.rfc-editor.org/rfc/rfc-index-latest.txt),
and the crucial [IANA protocol registries](https://www.iana.org/protocols) 
that provide the connective tissue binding the modern
Web.  Finally, the w3c's [Design Issues](https://www.w3.org/DesignIssues/)
notes collected by Tim Berners-Lee provides insight into
the thinking behind design decisions for the Web.

The design implications published here draw from 
the sources above.  In many cases, the conclusions
may run counter to popular API design practice.  
These cases exemplify differences between the
popular notion of REST, which may be better
termed [ROSI](https://restful-ws.github.io/rest/rosi).  These cases offer an
opportunity to explore REST's nuance and the
tradeoffs taken with varying interpretations of
the source material.

### Common Web API Producer Process

Before exploring REST's implications, it is worthwhile
to discussion the current state of Web API design.

#### The Primacy of OpenAPI
Outpacing competing Web API specification formats,
the [OpenAPI](https://www.openapis.org/) 
specification format has emerged as
the primary design document for Web APIs.  OpenAPI
captures and expresses key API details, including
tempalted resource identifiers, headers, parameters,
media types and schemas.  It promotes reuse
of element definitions. Having an OpenAPI
definition is widely considered to be an 
essential component of any mature Web API
definition.

OpenAPI's widespread adoption has been due,
at least in part, to its role in enabling a
robust tool ecosystem.  Most firms make
use of OpenAPI editors to assist in hands-on
design. Developer portals render API
documentation directly from the specification.
Test tools readily accept the format.
OpenAPI can also power server code 
generators, client code generators for SDKs, 
and linters, which spot quality issues.

#### API as a Product
As firms have begun to recognize the importance
of APIs in their digital transformation and
their integrated services offerings, many have
shifted to an _API as a Product_ approach.
Organizations have begun applying the tools
and practices of _Product Management_ to API
design and delivery.  Now, product managers
assess the market value of APIs,
define anticipated monetary flows, assess
strategic fit, produce product requirements,
manage product development, perform
go-to-market activities, and direct
other product lifecycle activities for
the API.

#### API Gateways
_API Gateways_, which centralize an
organiation's API exposure and management
activities, have become a common fixture
for API-enabled firms.  These provide
a wide variety of benefits, providing
opportunities for consistency across
security, logging, metering, reporting,
planning, and governance.   

#### The Typical Process

Organizations following a typical
API producer process organize their
API efforts into products, relying
on a Product Manager and an Agile
development management process.

1. The Product Manager performs the 
necessary work to determine that the 
product is work the investment.
2. The Product Manager produces
requirements for the API.  These
often come in the form of user 
stories.
3. The product manager
and technical organization perform
analysis of the stories.  They may
drawing from any existing domain 
driven design materials or enterprise
information models if they
exist.  They may produce candidate
resource definitions, URI templates,
operations, and schemas.
4. The product manager works with
an architect or development lead to
craft a _draft OpenAPI specification_.  
The specification includes candidate
endpoints and operations.
5. The API specification is presented
to stakeholders, both consumers and producers
of the intended API, as well as 
organizational API governance,
for feedback.  The
specification is updated based on the
feedback.

6. The delivery team develops the
API gateway configuration, the API 
origin service, and undertakes 
testing.  The team iterates through
stories, adjusting and correcting as 
problems are presented.  They also
make the linkages required for
operational readiness.  API Developer
documentation is prepared.

7. Product commercialization activities occur
in parallel to development.

8. The Web API product is launched.
API consumers, typically 
 _software developers_, use the firm's
Developer Portal to learn how to
interact with the API.  In many cases,
they will use an OpenAPI Specification
and off-the-shelf tooling to improve
consistency or speed their work.

10. The Product Manager performs standard
product lifecycle activities: measuring,
reporting, and managing product changes
through agile.  If the changes are
significant, they may warrant a return
to earlier steps.

#### Weaknesses in Common Producer Process?

Counterintuitively, through the lense of REST
and modern, there are a number of problems in
common practice. 

Inappropriate Client-Server Relationship
: Sharing URI templates with client developers
breaks design independence. This tight coupling
undermines independent evolvability. (See ROSI)

Inadequate Self-description
: asdfa

API-centric, rather than Resource-Sentric Schemas
: abc





### The Client-Server Relationship

URI Opacity: Clients do not read URIs.



### Component Independence

#### Independent Evolvability

#### Use-time Loose Coupling

#### Design-time Loose Coupling


### Resource Orientation

#### The Structured URI

#### The Opaque URI


### Client Competence

#### Independent Evolvability


