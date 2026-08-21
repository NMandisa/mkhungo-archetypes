# Mkhungo Maven Archetypes

A collection of custom Maven archetypes created to standardise and accelerate the creation of Java enterprise application projects.

The project captures reusable application starting points based on common enterprise development scenarios, including:

* Enterprise Edition applications
* Hibernate persistence
* Spring and Hibernate integration
* REST services
* Multi-module Maven projects
* Traditional Java web applications

Rather than repeatedly creating the same project structure and baseline configuration, each archetype provides a reusable starting point that can be generated using Maven.

---

## Why This Project Exists

When building multiple Java applications, the initial setup work can become repetitive.

Projects often begin with many of the same foundational decisions:

* Maven coordinates
* Package structure
* Dependency configuration
* Build configuration
* Persistence setup
* Spring configuration
* Web application structure
* Module boundaries

**Mkhungo Maven Archetypes** was created as an exploration into turning these recurring engineering decisions into reusable project templates.

The objective is not to eliminate architectural decision-making, but to reduce repetitive bootstrap work by capturing common application structures that can serve as a starting point for new projects.

> Reusable structure should reduce repetitive setup work while leaving project-specific design decisions to the application being built.

---

## What Is a Maven Archetype?

A Maven archetype is a reusable project template.

Instead of manually creating a project directory, configuring a `pom.xml`, creating the package structure, and adding common baseline files, an archetype can generate a new project from a predefined structure.

Conceptually:

```text
Developer
    │
    ▼
Select Archetype
    │
    ▼
Provide Project Coordinates
    │
    ▼
Generated Project
    │
    ├── Maven Configuration
    ├── Package Structure
    ├── Source Structure
    └── Baseline Configuration
```

This repository explores how Maven archetypes can capture reusable application structures for common Java enterprise development scenarios.

---

## Archetypes

| Archetype                            | Purpose                                                               |
| ------------------------------------ | --------------------------------------------------------------------- |
| `mkhungo-ee-archetype`               | Baseline template for Java Enterprise Edition applications            |
| `mkhungo-hibernate-archetype`        | Starting point for applications requiring Hibernate-based persistence |
| `mkhungo-spring-hibernate-archetype` | Template combining the Spring Framework and Hibernate                 |
| `mkhungo-rest-archetype`             | Baseline structure for REST-oriented Java services                    |
| `mkhungo-multi-module-archetype`     | Starting point for Maven projects composed of multiple modules        |
| `mkhungo-webapp-archetype`           | Template for traditional Java web applications                        |

Each archetype represents a different application bootstrap scenario and can be used as a reusable foundation for further development.

---

## Engineering Motivation

This project reflects an interest in **repeatability, standardisation, and reusable software structure**.

As enterprise applications grow, teams often establish conventions around:

* Application structure
* Dependency management
* Persistence configuration
* Module organisation
* Framework integration
* Build tooling

This repository explores a simple engineering question:

> **Can recurring application structures be captured as reusable development starting points?**

The result is a collection of Maven archetypes representing different Java enterprise application scenarios.

The broader principle is that repeatable technical decisions can be standardised, while application-specific design and architectural decisions should remain intentional.

---

## Repository Structure

```text
mkhungo-archetypes/
│
├── mkhungo-ee-archetype/
├── mkhungo-hibernate-archetype/
├── mkhungo-multi-module-archetype/
├── mkhungo-rest-archetype/
├── mkhungo-spring-hibernate-archetype/
└── mkhungo-webapp-archetype/
```

Each module represents an independent Maven archetype targeting a different Java application scenario.

---

## Building the Archetypes

Clone the repository:

```bash
git clone https://github.com/NMandisa/mkhungo-archetypes.git
cd mkhungo-archetypes
```

The archetypes can then be built and installed locally using Maven:

```bash
mvn clean install
```

Once installed, the archetypes can be used as local templates for generating new Maven projects.

---

## Engineering Context

These archetypes were developed as practical experiments around recurring Java enterprise application structures.

The repository is particularly relevant to developers working with traditional enterprise Java ecosystems involving:

* Maven
* Java Enterprise Edition
* Spring Framework
* Hibernate
* RESTful services
* Multi-module applications
* Traditional Java web applications

The project is less about generating applications automatically and more about exploring how recurring structural decisions can be formalised into reusable development assets.

---

## Project Status

This repository is an experimental collection of custom Maven archetypes.

It represents an exploration of:

* Java project standardisation
* Maven archetype development
* Reusable application scaffolding
* Enterprise application structure
* Build and dependency management
* Repeatable development foundations

The archetypes are maintained as development and learning artifacts and may be expanded, modernised, or refined over time.
