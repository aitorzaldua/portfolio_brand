---
title: How Microsoft is Adopting Rust
description:  Microsoft determined that 70% of security patches pushed to computers are to fix memory-related bugs and believes that Rust would’ve been able to catch these bugs during the development phase
---

![](/img/microsoft.jpeg)

Microsoft has one of the largest C/C++ codebases in the world. All of its core products from Windows and Office to the Azure cloud run on it. Unsurprisingly, since C++ is not a memory-safe language, a lot of memory bugs popup in their codebase, and a lot of time has to be spent fixing them. Last year, Microsoft began looking at alternative programming languages that could help fix their memory safety issues. As a result of these pursuits, Microsoft has begun experimenting, and in some cases integrating, Rust into their codebase. Rust is a relatively new programming language that promises the same low-level performance of C and C++ with a feature set expected from a modern programming language. Microsoft thinks Rust has potential, and here is how they are integrating it into their products.

*Rewriting Windows in Rust.*

Ok, they aren’t rewriting all of Windows in Rust just yet; but, they are interested in seeing how Rust will fit into its ecosystem. Microsoft determined that 70% of security patches pushed to computers are to fix memory-related bugs and believes that Rust would’ve been able to catch these bugs during the development phase. As a result, they tasked some engineers to rewrite some components of Windows in Rust to get some developer sentiment.

Microsoft has unfortunately kept the name of the components being rewritten secret, however, one engineer described that he was working on a “low-level system of Windows.” This shows the faith Microsoft has in Rust’s potential. They aren’t just looking to rewrite some of their small services or native Windows app, but possibly core components of the operating system.

The engineers described their work with Rust as “generally positive” but did note that some important features available in C were missing for Rust. The engineers, however, do think that it’s worth helping to develop such features for Rust. Intel has already begun working on bringing Rust to feature-parity with C, and Microsoft could join them on this effort. Since some features of C are missing from Rust, the team found that Rust will be best suited for new or recently-developed Windows components. It wouldn’t be surprising if Microsoft fully committed to migrating part of their codebase to Rust. They’re already building a standard Windows library for Rust that will have all of the capabilities of the C++ version. Linux is also considering migrating some of its kernels over to Rust, so I wouldn’t be shocked if a race sprung up between the two operating systems to see which one could push Rust code to production first.

*Incorporating Rust into Azure services*

DeisLabs, one of Azure’s incubators, focuses on building tools for Kubernetes and recently chose Rust to build their new product Krustlet, a service that allows developers to run multiple WebAssembly modules in Kubernetes. Kubernetes was developed by Google and written in Go. As a result, most engineers tend to stick with Go when writing their Kubernetes components, so it’s quite surprising that DeisLabs chose Rust.

In the end, the decision seemed to pay off. While employees did note that the shift to Rust was difficult — noting the uniqueness of Rust’s ownership philosophy — it only took the team a month to return to full efficiency. They found that they were writing fewer tests for null values and debugging fewer problems. The engineers were also impressed by Rust’s compiler, which they claim would’ve caught security flaws found in another one of their projects that Go’s compiler failed to find. They concluded that more teams should consider working with Rust in the future and that it could be better suited for Kubernetes development than Go.

*A new programming language*

A little while ago, Microsoft had investigated creating their programming language inspired by Rust. One of the leaders of the project is the primary maintainer of C#, so it seems likely that the language is a version of Rust with syntax more similar to the C-family of programming languages. This language, dubbed Project Verona, is aimed to address memory-related bugs in systems programming. Some speculate that Project Verona could eventually find its way into a lot of major Microsoft products, such as Windows, Xbox, and Azure.

Ultimately, Microsoft still doesn’t have any use-cases for Project Verona. They do claim that the language is already “completely memory safe.” However, Microsoft remains in favor of using Rust instead. It already has a community and the support of companies like Mozilla and Intel. Joining forces with those companies would allow Rust to become much more powerful much quicker.

The future is very bright for Rust. With large companies backing it and a growing community, it has a very promising future. It wouldn’t be surprising to hear over the next couple of months the different ways Microsoft plans to incorporate Rust into its company. Rust is also well-optimized for microcontrollers and IoT devices, and we can expect to hear the use-cases companies in these spaces have found for Rust.

[Read the original post here](https://medium.com/@tinocaer/how-microsoft-is-adopting-rust-e0f8816566ba)