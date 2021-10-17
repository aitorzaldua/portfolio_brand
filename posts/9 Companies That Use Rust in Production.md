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

[Figma](https://www.figma.com/) is a collaborative web-based design tool for vector graphics and interface prototyping. They chose to rewrite their multiplayer syncing engine in Rust (previously, it was in TypeScript) to improve performance since their server couldn’t keep up with user growth.

We chose Rust for this rewrite because it combines best-in-class speed with low resource usage while still offering the safety of standard server languages. Low resource usage was particularly important to us because some of the performance issues with the old server were caused by the garbage collector. [(Source)](https://www.figma.com/blog/rust-in-production-at-figma/)

Find out more about their use of Rust in this article on [Rust in production at Figma.](https://www.figma.com/blog/rust-in-production-at-figma/)

## npm










[This post was originally posted by devgenius](https://blog.devgenius.io/9-companies-that-use-rust-in-production-9b8f6634b7b4)