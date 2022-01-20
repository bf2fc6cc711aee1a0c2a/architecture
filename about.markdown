---
layout: page
title: About
permalink: /about/
layout: default
---

# Document types

This pages describes the different kinds of content on this site.

## Architecture Overview

### Audience

* External stakeholders
* People new to the project
* Anyone looking for a refresher on the general architecture

### Description

A living document that serves as an introduction and jumping off point for the managed service architecture. High level overview of the key contexts and components. Should link off to more detailed context overviews and also any key overarching ADRs. Should be kept high level to minimize the maintenance cost.

### Process

Updating the Architectural overview is a step part of an ADR or an Epic Brief elaboration.



## Context Overview

### Audience

* External Stakeholders 
* New people joining the team particularly if working in a particular context
* Team members working in other contexts that want a better and deeper understanding of a particular context
* Anyone looking for a refresher on a particular context

### Description

Living document that is a focused and detailed architectural overview of a particular context. Example contexts would include the Control Plane and Data Plane. Should outline each of the components in that context (including important if not all sub components. Key interactions should also be outlined with a reasonable amount of detail while avoiding implementation details where possible. Should be kept high level to minimize the maintenance cost.

### Process

Updating the Context overview is a step part of an ADR or an Epic Brief elaboration.



## Architecture Decision Records (ADR)

### Audience

* Architects / Team Leads / Engineering from all services

### Description

Captures single important architectural decisions including the why and what but should avoid implementation details where possible that may soon become out of date or not apply to other services that want to follow the decision made in the ADR. ADRs should be addressing how to solve a problem, their title reflecting it. Other service teams would reuse these cookbooks. 

### Process

It is expected that ADRs will be matured within an Epic Brief: while working on the technical aspect of an Epic Brief, the ADRs will be identified and moved to an appendix while maturing the solution. ADRs can then be extracted as a separate document.
An ADR :

* Is recorded in the [ADR index](/ADRs)
* follows the [ADR template](/adrs/000/Defining_a_template_for_architecture_Decision_Records.html)
* lives under the `_adrs` directory of this site.
* Is announced to mas-architecture@redhat.com
    - When identified
    - When proposed to move to accepted
* Is announced to mas-all@redhat.com
    - When accepted  



## Epic Brief

### Audience

* Architects / Team Leads / Engineering
* BU and PM

### Description

Focused design doc that dives into the details of how to execute on a given solution to the outlined problem. The problem will have often been posed by PM and would include user stories along with the proposed solution. The document is considered stale as soon as the Epic Brief has been delivered.

### Process

Often an epic brief will be one of the first documents created by the engineering team and serves as a point of discovery for new Architecture Decision Records. Forming the basis of a new ADR within an epic brief before extracting it out is a process that is highly encouraged to reduce mental overhead. For example by dedicating an appendix section per ADR and mature it as part of the Epic Brief process.

It is critical that as part of an Epic Brief, existing ADRs are reviewed to see what can be reapplied, new ADRs are identified and extracted and that any architecture impacting conversation are flagged for architects to look at. For the latter, an email to mas-architecture@redhat.com pointing to a bookmark URL is the preferred mode.



## Component-level Design Documents

### Audience

* Team Leads / Team members

### Description

* Detailed description of how the different layers of a single component fit together. Key areas in the code and key design decisions that have influenced the structure and design of the code. 

### Process

This document will live close to the code (same repository).