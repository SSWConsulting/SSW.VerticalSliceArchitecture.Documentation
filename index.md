---
_layout: landing
title: Home
---

# Vertical Slice Architecture

Originating in 2018 by Jimmy Bogard, through [this blog post](https://www.jimmybogard.com/vertical-slice-architecture/) & this [NDC presentation](https://www.youtube.com/watch?v=SUiWfhAhgQw) Vertical Slice Architecture (VSA) has been making waves in the .NET community. It's a great way to have a highly cohesive codebase & deliver features quickly in an enterprise environment.

The most dominant (and highly controvesial - at least online) architecture, Clean Architecture is the go-to for many organisations for it's great promises of maintainability and testability. However, it's not without it's drawbacks. But, more accurately, it's not the best choice for every project (i.e. the golden hammer).

The most immediate difference between these two, is:

- Clean Architecture favours a layered approach, where each layer is a **technical** concern.
- VSA favours a feature-based approach, where each feature is a **business** concern.

## What is this?

This is the best place to [learn](~/learn/overview.md) about Vertical Slice Architecture (VSA).

- You can find [samples](~/samples.md) of real apps that use VSA.
- You can find curated external [media](~/media.md)

There isn't much online in terms of VSA, so I'm hoping to change that (there are a lot of repetition of the same ideas). Both, by articulating the theory and by providing practical examples.

The site is primarily a knowledge base for VSA, but the code examples are for .NET/C#, typically thinking about a Web API on the ASP.NET Core engine. This is done using a companion [VSA Template]() that I maintain. The template, importantly, should *not* be the starting point. It is a tool to bootstrap the theory learnt here.

## I'm lost, help me!

> [!TIP]
> If you're unfamiliar with common architectures, I have a quick primer presented at .NET Conf 2023. It walks through a progression from Spaghetti architecture to Clean Architecture, and then to VSA.
> 
> > [!Video https://www.youtube.com/embed/T-EwN9UqRwE]

## An important note

This site is a new work in progress. If you have any feedback, please create a new [issue](https://github.com/Hona/VerticalSliceArchitecture.Documentation/issues) or [discussion](https://github.com/Hona/VerticalSliceArchitecture.Documentation/discussions).

> [!NOTE]
> This is my personal opinion and not the only way to implement VSA. 
>
> While it's a living document & will evolve with the community, you might disagree with some of the content. 
> I encourage you to create a discussion, as I'm always open to learning new things.