---
layout: default
title: Misconceptions
permalink: /rest/constraints/misconceptions
---

## Misconceptions about REST

Despite widespread use, REST is a source of
confusion for many practitioners, especially
those working on Web APIs.

One can spot the confusion by looking for 
a few telltale signs.

1. Do changes to the API break the client?

REST was design to avoid tight coupling 
between client and server.  Web components
are intended to evolve independently!
The RESTful Web is so flexible, so 
resilient, so graceful in the face of
unexpected responses and change.  But solutions based on
REST APIs seem so brittle; an
unexpected field change can break
the client.  

Why are APIs Programs so concerned
about API versioning? Why would seemingly 
minor changes be so impactful?  Are there
differences between the browsable Web 
and the typical REST API client?

2. Is the API provider sharing URIs with
the API consumer?

Does the API provider expect the API
consumer to tightly couple its 
client to specific URIs?

Is the API client expecting to infer
a JSON or XML schema based on which
it used to access the representation?

3. Does the API use base structured
syntax media types as the media types
for its representations?  Does the
provider use `application/json`,
`application/xml`, rather than using
a named media type with a 
structured syntax suffix,
`application/fancy-resource+json`?

4. Does the API avoid using links?

Some APIs provide identifiers that
indicate the type of link or the
media type of the target resource.
Others merely provide opaque, non-URI
identifiers that point to the related
resource.  In either of these cases...



## TBD content
...


In a world of OpenAPI specification sharing,
directing API consumers to endpoints and
methods is the norm.  But when a client
is written to integrate with specific
endpoints, rather than those that they
learn in the course of interacting with
the authority and resource, they
steer away from REST and its constraints.



