---
title: 'Visualising your architecture using the C4 Model'
description: ''
pubDate: 'Feb 3 2023'
draft: true
heroImage: '../../assets/blog/c4-model.png'
tags:
  - 'architecture'
  - 'modelling'
  - 'C4'
---

The adoption of agile software development practices has seen the method of documenting solutions in large, up-front, detailed documents with great scepticism. But projects are fast-moving, team members come and go, and the knowledge they have of the architecture or system can go with them.

While there are numerous diagramming tools out there like ArchiMate and UML, many can be dauntingly intricate. Have a look at the number of pages in the hardback textbook provided by ArchiMate. Of course, you could invest time and resources into mastering these frameworks, but I have found the C4 model is a solution that shines through as a ray of hope for any software architect or designer.

C4 diagrams are an efficient way to visualise software architecture and provide a clear, concise and consistent way of communicating the design of a software system. They are increasingly being used as a standard for software architecture documentation, and for good reason.

One of the key benefits of C4 diagrams is that they are easily understandable by non-technical stakeholders. This makes them ideal for communicating the design of a software system to stakeholders who may not be familiar with technical jargon. C4 diagrams provide a high-level overview of the architecture of a system and can be used to convey the overall structure, context, and key components of a system.

## The four levels of C4

### Level 1: Context

The Context level is the bird's-eye view of your system. At this level, you show how your system fits into the bigger picture, defining the boundaries and the system's primary responsibilities. Here you identify and document users (or actors) and the external systems that your software interacts with. A context diagram can illustrate the high-level flow of data and highlight the major dependencies and interactions.

### Level 2: Containers

Delving deeper, the Container level breaks down the system into its top-level containers like web servers, databases, mobile apps, desktop apps, etc. Each container embodies an application or data store. This level is crucial for developers and operations as it lays the foundation of the tech stack and the way different applications interact.

### Level 3: Components

At the Component level, each container from the previous stage is further broken down into smaller, more manageable parts. These parts or components represent different functional areas or classes. It provides a closer look at the inner workings of each container, which aids developers in understanding how each part collaborates with the others.

### Level 4: Code

The most granular level, Code, dives deep into each component's innermost workings. Here, we explore how components are implemented, usually using UML class diagrams or similar tools. This level is most beneficial for developers actively working on or maintaining the codebase.

## Supplementary diagrams

### System Landscape diagram

The System Landscape diagram provides a broader view of all systems (not just the primary one) in an environment and how they interconnect. It’s valuable for architects and stakeholders to understand the overall ecosystem.

### Deployment diagram

This diagram displays how software components reside on hardware. It provides a map of where each part of your system lives, which is invaluable during deployment, troubleshooting, and infrastructure planning.

## Living Documentation

In the context of software architecture, C4 diagrams can serve as living documentation by providing a clear, concise, and consistent way of communicating the design of a system. They can be updated and revised as the system evolves, allowing the architecture to evolve with the system. This makes it easier to keep track of changes over time and to ensure that everyone has a clear understanding of the design.

### Notes

-   I have introduced the C4 model in several products and enterprise projects. In some of these projects in which I am no longer involved, the documentation lives on and provides developers and architects with a shared understanding of what exists, and gives them the ability to continue to update and communicate changes as the software system continues to evolve.
-   C4 does not replace other diagramming tools such as UML or ArchiMate. Indeed, UML can be incorporated into level 4 of C4 if the documentation would benefit from it.
-   Codifying C4 using apps like Structurizr is beginning to have traction. However, it's far from being a necessity in your modelling.
-   I have lambasted ArchiMate for producing a large hard-backed book. Yet, I'm advocating for an alternative for which the creator, Simon Brown, has written **two** books. Granted, neither breach 100 pages when put together. I don't think you need the books either.

### Links

-   C4 model website: [https://c4model.com](https://c4model.com/)
-   Templates for [LucidChart](https://www.lucidchart.com/pages/templates/c-4-model-example), [Visio](https://github.com/pihalve/c4model-visio-stencil), [draw.io](https://www.diagrams.net/blog/c4-modelling), and [Miro](https://miro.com/miroverse/c4-architecture/)
