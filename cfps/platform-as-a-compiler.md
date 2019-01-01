# Title
Platform as a Compiler: How can FaaS platforms optimize code

# Elevator Pitch (300 characters)
Modern compilers and processors optimize execution performance using techniques like branch predictions and code inlining. Can FaaS platforms utilize static and dynamic analysis for FaaS performance optimization?

# Talk Format
40 minutes

---

# Description

Developers in compiled languages like Java and C rely heavily on compiler performance optimizations. These optimizations help developers express business logic in their code, rather than speed tricks.

Cloud developers are not that lucky. Functions on FaaS platforms are frequently written in interpreted languages, and suffer from performance characteristics order of magnitude slower than compiled code.

In this session I will review a few code optimization techniques used by compilers, like branch prediction and code inlining, and a few error handling techniques like stack traces and exception mechanisms. For each mechanism, I will present an equivalent FaaS optimization technique that can greatly improve the execution path performance. I will argue that these techniques should be part of FaaS platforms in the near future, but we can easily implement some common patterns today to gain 
a 80-20 performance improvement. 

# Topics covered
* Intrducing the problem: FaaS latency, typical metrics and function composition
* [Branch prediction](https://stackoverflow.com/questions/11227809/why-is-it-faster-to-process-a-sorted-array-than-an-unsorted-array): Predictive function calls by critical path analysis.
* [Code inlining](https://en.wikipedia.org/wiki/Inline_expansion): How to inline FaaS calls to reduce latency. Principle of least privilege and function security scope; Manual, CI/CD, and platform based inlining.
* [Stack Traces](https://en.wikipedia.org/wiki/Stack_trace): How to build a cloud stack trace, analogous to a local stack trace.
* [Short-circuit evaluation](https://softwareengineering.stackexchange.com/questions/371832/when-is-short-circuit-evaluation-bad) and [concurrency operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/all) with cloud functions.

# Is it practical?
_Yes_. Even though not every technique presented in this session is supported by platforms or third-party tools out of the box,  all of them can be applied at the developer level without outside tools.

# Is it vendor-specific?
_No_. It's a general architectural and design session. All the techniques reviewed in this session are applicable to any cloud vendor or on-prem FaaS platforms.

![Railroad branch](https://upload.wikimedia.org/wikipedia/commons/c/cf/Entroncamento_do_Transpraia.JPG "By Mecanismo [CC BY-SA 3.0  (https://creativecommons.org/licenses/by-sa/3.0)], from Wikimedia Commons")

---

# Notes for the reviewers

