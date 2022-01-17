---
layout: default
title: What is ROSI?
permalink: /rest/rosi
---

## ROSI: Resource Oriented Service Integration

**ROSI** is a term for a popular style of Web API design.  It
is derived from REST, the architectural style published
by Roy Fielding, but differs in key areas.  By relaxing 
some of REST's requirements, ROSI forfeits some of
REST's advantages while providing design-time benefits
to Web API and client producers.

| Constraint                                          | REST     | ROSI                                       |
|-----------------------------------------------------|----------|--------------------------------------------|
| Client-Server                                       | Required | Use Time                                   |
| Stateless                                           | Required | Soft Requirement                           |
| Caching                                             | Required | Syntactical Support, Optional to Implement |
| Uniform Interface                                   | Required | Required                                   |
| / Resource Identification                           | Required | Required                                   |
| / Manipulation of Resources through Representations | Required | Required                                   |
| / Self-descriptive Messages                         | Required | Soft Requirement                           |
| / Hypermedia (As the Engine of Application State)   | Required | Not Required                               |
| Layered System                                      | Required | Required                                   |
| Code On Demand                                      | Optional | Optional                                   |


**ROSI** solutions and APIs are resource-oriented.  Request and responses
always occur in the context of an _identified resource_.
Like REST, the nature of the resource can be anything.



