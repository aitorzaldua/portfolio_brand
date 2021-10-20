---
title: 9 Companies That Use Rust in Production
description: Who uses Rust, and what are the benefits of choosing this programming language for your stack?
---
![](/img/fot7.jpeg)

If you haven’t yet heard, Rust is one of the most promising and most loved programming languages out there.

First created at Mozilla, it has since been adopted by companies like Dropbox, Microsoft, Facebook, and others. Rust’s main benefit is that it enables C-like performance while still keeping the memory safety that we are used to when developing with languages like JavaScript and Python.

In this article, I will look at nine large companies that use Rust and delve into the reasons for their choice.

## 9 Rust success stories

### Dropbox

![](/img/dropbox.jpg)

[Dropbox](https://www.dropbox.com/) uses Rust for parts of its file synchronization engine. Since the engine is highly concurrent, writing, testing, and debugging it is hard. Therefore, the team chose to rewrite it in Rust. Rust’s static types and heavy compile-time checks give it an advantage over dynamically typed languages like Python when you need to tackle complex codebases and concurrent code.

Rust has been a force multiplier for our team, and betting on Rust was one of the best decisions we made. More than performance, its ergonomics and focus on correctness has helped us tame sync’s complexity. We can encode complex invariants about our system in the type system and have the compiler check them for us. [(Source)](https://dropbox.tech/infrastructure/rewriting-the-heart-of-our-sync-engine)

Read more about Dropbox’s use of Rust on [their tech blog.](https://dropbox.tech/infrastructure/rewriting-the-heart-of-our-sync-engine)

### Coursera

[Coursera](https://www.coursera.org/) uses Rust for their programming assignments feature where students need to write and run a computer program to solve a problem. The programs are run, tested, and graded inside Docker containers. For security reasons, the developer team needed to use a low-level language like Rust for some of the code, and they decided that Rust is more secure than C.
Although C is the default low-level full-control programming language, these binaries have strict security and correctness requirements. We instead have chosen Rust, a modern native language from Mozilla. One of Rust’s common selling points is complete immunity to certain classes of security vulnerabilities thanks to its powerful type system, making it an excellent choice for security critical functions. [(Source)](https://medium.com/coursera-engineering/rust-docker-in-production-coursera-f7841d88e6ed)

You can get more details on their use of Rust for programming assignments [on their blog](https://medium.com/coursera-engineering/rust-docker-in-production-coursera-f7841d88e6ed).

### Figma

![](/img/figma.jpg)

[Figma](https://www.figma.com/) is a collaborative web-based design tool for vector graphics and interface prototyping. They chose to rewrite their multiplayer syncing engine in Rust (previously, it was in TypeScript) to improve performance since their server couldn’t keep up with user growth.

We chose Rust for this rewrite because it combines best-in-class speed with low resource usage while still offering the safety of standard server languages. Low resource usage was particularly important to us because some of the performance issues with the old server were caused by the garbage collector. [(Source)](https://www.figma.com/blog/rust-in-production-at-figma/)

Find out more about their use of Rust in this article on [Rust in production at Figma.](https://www.figma.com/blog/rust-in-production-at-figma/)

## npm

[npm](https://www.npmjs.com/) is a package manager for JavaScript. Its engineering team chose to rewrite their main service in Rust because they saw that the service’s performance would soon be a bottleneck if user growth kept up. They rejected technologies such as C and C++ since they didn’t trust themselves to be able to handle memory management for a web-exposed service. Java was rejected since it would involve deploying JVM on their servers. 🙃

The challenges that npm faces demand efficient and scalable solutions. When a service can be deploy-and-forget, that saves valuable operations time and lets them focus on other issues. npm employees also value having a helpful community around any technology they use. Rust fits all these criteria and is currently in use as part of npm’s stack. [(Source)](https://www.rust-lang.org/static/pdfs/Rust-npm-Whitepaper.pdf)

To learn more, read their [case study](https://www.rust-lang.org/static/pdfs/Rust-npm-Whitepaper.pdf) on Rust’s homepage.

## Microsoft

![](/img/micros.jpg)

Microsoft has recently been experimenting with integrating Rust into its large C/C++ codebases.

The main argument for adopting Rust at Microsoft was the memory safety that Rust provides. For the last 12 years, around 70 percent of the CVEs (Common Vulnerabilities and Exposures) discovered at Microsoft have been connected with memory safety. Microsoft has tried various options to solve this issue, such as extensive developer training and static analysis tools. However, it seems like the only way out is to make these vulnerabilities impossible to do.

## Cloudflare

Cloudflare uses Rust in their core edge logic and as a replacement for C, which is memory-unsafe.

Their [GitHub](https://github.com/cloudflare) shows 18 open-source repositories that use Rust, and on their blog, they document using it for Firewall Rules, a very customizable firewall tool.

With a mixed set of requirements of performance, memory safety, low memory use, and the capability to be part of other products that we’re working on like Spectrum, Rust stood out as the strongest option. [(Source)](https://blog.cloudflare.com/building-fast-interpreters-in-rust/)

## Facebook

![](/img/fcbook.jpg)

Facebook used Rust to rewrite its source control backend, which was written in Python. They were looking for a compiled language to rewrite it in and were attracted to Rust because of its safety benefits. Since then, Rust has been adopted by the source control team. As the reasons for adoption, they mention the huge cost of bugs for Facebook and the ease of the compiler feedback loop, in contrast to static analysis and code reviews.

Rust detects large classes of serious bugs at compile time. The cost of a bug at compile time is orders of magnitude less than in production.

## Amazon

[AWS](https://aws.amazon.com/) has used Rust for performance-sensitive components of services like Lambda, EC2, and S3. In addition, the company openly supports and sponsors the development of the language and its ecosystem.

Amazon also has open-sourced a service written entirely in Rust. [Firecracker VMM](https://firecracker-microvm.github.io/) is a virtual machine monitor that was built for services like AWS Lambda and AWS Fargate.

## Discord

![](/img/discord.jpg)

[Discord](https://discord.com/) uses Rust in multiple places of their codebase, both on the client- and the server-side.

For example, the team used Rust and [Elixir](https://serokell.io/blog/introduction-to-elixir) to scale to 11 million concurrent users through the use of Elixir NIFs (Native Implemented Functions). In this case, Rust enabled them to speed up their existing Elixir codebase while keeping everything memory safe.

They have also rewritten their Read States service in Rust (originally in Go). While the Go version of the service was fast enough most of the time, it sometimes had large latency spikes due to Go’s memory model and garbage collector.

To solve that, Discord switched to Rust, which offers a unique memory allocation system that makes garbage collection unnecessary.

Along with performance, Rust has many advantages for an engineering team. For example, its type safety and borrow checker make it very easy to refactor code as product requirements change or new learnings about the language are discovered. Also, the ecosystem and tooling are excellent and have a significant amount of momentum behind them. [(Source)](https://blog.discord.com/why-discord-is-switching-from-go-to-rust-a190bbca2b1f?gi=f6619f5a6d0f)

To read more about their use of Rust, check out this article on [their blog](https://blog.discord.com/why-discord-is-switching-from-go-to-rust-a190bbca2b1f).

## Future of Rust

In most of these companies, Rust functions as a strictly better alternative for C — you can see a visible pattern of rewrites done in Rust to escape performance degradation. Teams reach for it when they need extra performance but want to avoid memory issues associated with C.

But Rust has far more benefits: it makes lower-level programming more accessible, has excellent support for WASM, and is fantastic for concurrency. And I’m not even going to start to speak about the community. ❤️

In the future, expect Rust usage to increase as more and more companies discover how it can improve their codebases.



[This post was originally posted by devgenius](https://blog.devgenius.io/9-companies-that-use-rust-in-production-9b8f6634b7b4)