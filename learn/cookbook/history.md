<!-- 2018 is in the home page. But, there is stuff as early as 2015 called 'SOLID Architecture' which is basically his VSA stuff -->

# History

Architecture is a certainty in software development. There have been many architectures over the years, and you can find a plethora of information on Google.

The history of just Vertical Slice Architecture is a bit more recent. The term was coined by Jimmy Bogard in 2018. However, the ideas behind it have been around for a while. 

## 2015

In fact, [as early as 2015](https://vimeo.com/131633177), Jimmy was talking about SOLID Architecture which is essentially the same thing. It had a few key points (from his slides):

> - SRP - One class per feature/concept
> - OCP - Extend through cross-cutting concerns
> - LSP - Just don't do inheritance
> - ISP - Separating queries from commands
> - DIP - Save for true external dependencies.

The key points of the SOLID architecture were really applying the principals to achieve a highly cohesive codebase in regard to the Domain specific code (SRP, ISP). The Domain specific code was then extended (OCP) via cross-cutting concerns - like authentication, authorization & generic logging. 

A lot of the outcomes from this talk to me, was allowing a simpler architecture for what matters most - the Domain. The most important thing in software, is that it works. The architecture that allows you to deliver features quickly, is the best architecture for you.

## 2018

Moving along a few years, in 2018, Jimmy wrote a blog post called [Vertical Slice Architecture](https://www.jimmybogard.com/vertical-slice-architecture/). This was the first time the term was used. It was then shortly followed up with [a presentation at NDC Sydney](https://www.youtube.com/watch?v=SUiWfhAhgQw) later that year.

The key points of this evolution of the architecture were (from the presentation):

- CQRS - e.g. HTTP GET is safe & idempotent, POST is Unsafe & not idempotent. Represent this two different concerns in different models/classes where this was just one.
- Vertical Slicing makes it easy to modify code
- Do not skip the refactor step in Red-Green-Refactor. (Common complaints about 'simple' architectures is due to this)
- Push behaviour down (i.e. Focus on a rich domain & allow handlers to do the 'ugly' work, like data access)
- Integration test handlers & unit test Domain

## Where it was left

At that point, Jimmy has set the world up with some pretty nice foundations.

1. Logically split application reads & writes using CQRS.
1. CQRS models are use cases. Application use cases should be sliced & tightly coupled within
1. Refactor repeated logic into a rich Domain
1. Refactor repeated domain-agnostic code into services, repositories
1. Integration test use cases
1. Unit test the Domain