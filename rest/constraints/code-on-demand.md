---
layout: default
title: Code On Demand Contraint
permalink: /rest/constraints/code-on-demand
---

## The _Code On Demand_ Constraint

Source
: Fielding Dissertation, [Section 5.1.7](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm#sec_5_1_7)

### The Constraint

The server may facilitate client processing by providing code to the client.

#### Defining Code on Demand

According to Fielding ([link](https://www.ics.uci.edu/~fielding/pubs/dissertation/net_arch_styles.htm#sec_3_4_3)):
> REST allows client functionality to be extended by 
> downloading and executing code in 
> the form of applets or scripts.

### Rationale

Code on Demands reduces the requirement to pre-implement every feature
required to support the application.  A client may gain features
through _late binding_ by obtaining the feature, via code,
when that code is needed.

## Observing Code On Demand in the Modern Web

- Javascript
- Java Applets
- Runtime Schema Delivery

## Implications of Code On Demand

TBD

### Implications of Code On Demand

XYZ
: TBD

## How to Mess It Up