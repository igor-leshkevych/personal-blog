---
title: Code analysis in .NET Core projects, Part 1
date: "2020-03-01T20:00:00.000Z"
description: Fast and reusable static code analysis setup for .NET Core with Roslyn analyzers
---

# Introduction (TODO: these are theses to use)

Code quality - attribute that usually introduces a gap between "business guys" and "tech guys". While other attributes are usually well understood by all parties (performance, correctness, security), code quality is something ephemeral - there is no an objective way to measure it, and for someone who is not directly involved in actual development it is not clear why business needs to spend time and money on refactoring/rewriting something that already works. 

While this gap deserves it's own article, let's focus more on code quality itself.

The evolution (timeline) of code quality perception:
- No quality (look old ASP.NET MVC repository for concrete example)
- Ad-hoc code reviews, enterprise code analysis tools (Sonar)
- Pull-requests
- Linters/formatters

Two ways to maintain code quality:
- Manual: code reviews, pull requests, code conventions
- Automatic: static code analysis, linters/formatters

There is a general trend in the coding industry of transferring more and more work from the developer's shoulders to machine: 
- Static type system
- Linters/formatters
- Automatic memory management aka Garbage Collection
- Container orchestrators

Two types of things we usually want to control:
- API design issues ("something bad might happen if you do that")
- Code conventions violation issues ("code is fine but is not consistent with other developers work")

To be continued ...

Part 1 is about #1, part 2 will be about #2