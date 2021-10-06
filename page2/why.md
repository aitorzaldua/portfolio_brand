---
title: 5 Reasons Why Rust Is The Future
description: Rust has its advantages over many languages that are currently well known to the developers. Let’s go over some of them. 
---

In the Stack overflow 2020 survey, Rust was picked as #1 most loved programming language, thanks to 86% of developers who said they would continue using it. For the language creators, this is nothing new – Rust has been winning the survey ever since 2016. On Tiobe Index, Rust is rising in popularity as well – achieving #18 positions among the most popular languages in September. It also didn’t fail in our own ranking of functional programming languages based on sentiment analysis gaining first place in the most positive sentiment class.

Created by former Mozilla developer Graydon Hoare in 2006 as an alternative to C++ language, Rust is slowly making a name for itself in the developers’ world. It’s now used to create web software, embedded computers, and distributed services or the command line. Suitable proof of that popularity is that worldwide giant Microsoft is slowly moving from C++ language (due to an ever-increasing number of security issues) to Rust.

Just what makes Rust so adored among the programmists, when they have so many other languages to use? One of the main reasons is that Rust solved many issues visible in different languages – to the point some developers say that the creators of Rust must have had all the potential problems visible in C++ in mind. What exactly makes Rust so unique, and is it worth it to learn Rust? Here are five reasons why we think Rust is our future.

**Rust vs other languages*

Rust has its advantages over many languages that are currently well known to the developers. Let’s go over some of them. 

*Rust vs C++: advantages*

Compared to C++, Rust is just… way safer. Rust protects both its own abstractions and the abstractions made by developers, while C++ lacks both of those options. Specific mistakes in C++ can lead to arbitrary behaviour whilst Rust helps you focus on what’s really important. And yes, C/C++ is still regarded as one of the most popular programming languages, yet it’s often leading to some problems. Rust is simply easier to approach, the learning curve is not very steep, there’s no technical debt in Rust as it is in C++, comes with easier concurrency, and the performance is comparative. Rust allows programmers to write unsafe code, but defaulting to safe code (if you opt-in, you can unsafe code in Rust with unsafe keyword – it comes by default with C++).

*Rust vs Java: advantages*

When it comes to Java, it turns out that this programming language is significantly slower than Rust, especially bearing in mind keeping up with C in many domains. Additionally, you need to bear in mind faster startup times and smaller memory footprint on top of it. Java uses Garbage Collection for memory management, which decreases performance (although it’s worth noticing that it makes programming easier).

*Rust vs Python: advantages*

Rust is well-designed. Rust allows for putting statements in a lambda and everything is an expression, so it’s easier to compose particular parts of the language. Python lacks it. Rust doesn’t have classes so the object orientation is not as evolved as it is in Python. Python also comes across with the necessity of writing more tests, production outages, or runtime crashes. Rust makes it less expensive to identify and fix possible bugs. 

*Rust vs Go: advantages*

Go lacks expressiveness. Rust has a flexible and expressive system that allows for defining new container types that can hold different types of elements, generics, traits, algebraic data types. Go gives you less control over both resources and memory. 

*Why is Rust the future?*

*1. Rust improved memory safety.*

One of the biggest issues that are plaguing the developers are memory management issues. It’s very easy to miss a code problem in other languages, which in turn gives dreaded error code – and demands time for finding and fixing them. A much bigger problem is when a coding mistake might cause security breaches – in today’s world, this is simply too dangerous. Loud cases of a data security breach in large and popular websites or apps happen far more often than we would like. The reason? Quite often, application vulnerabilities or misconfiguration.

Rust is considered to be memory-safe. Rust code cannot have any dangling pointers, buffer overflows or any other type of memory-related errors. It lets you define how the memory should be managed and how the values should be laid out in it, taking care of both the control and safety line without losing performance and making it a huge asset of Rust. 

Improving memory safety was one of Rust’s developers’ main goals and the language’s most significant selling points. Their code compiler is very strict, and each of the variables or memory addresses that are used are automatically checked. If there are any syntax errors, null values, dangling modifiers, or memory safety issues spotted, Rust won’t compile the code and warn about unsafe code that allows for quick spotting and fixing the main problem. How does it do that?

In Rust, every value has an “ownership.” When a value is passed or returned, the ownership is given to a new scope – and only one at a time. The value is then dropped if the “owner” of the value is moved out of the scope. That way, Rust keeps track of the memory and frees it automatically – and prevents all bugs from getting into the main code. That means no surprises at runtime! This system is to analyze memory management at compile-time, helping identifying and fixing bugs quicker and making garbage collection unnecessary. 

But there’s more about memory than that. Building advanced systems is often connected to heavily computation-bound work and creating A LOT of temporary memory. Such an offload can negatively affect any Java Virtual Machine performance and many programming languages – including Scala – simply cannot deal with it.

Yet, Rust can. It supports writing memory-efficient code, without managing memory or dedicating modern conveniences such as closures, and runs with minimal or no runtime overhead, being used for real-time or embedded projects, and easily integrating with other languages or projects. 

If this one hasn’t convinced you yet, let’s go further.

*2. Rust’s community keeps growing.*

Of course, Rust’s community and the number of libraries are nowhere near as big as, for example, C++. But with the growing popularity of the Rust language, the amount of developers and passionate people getting onboard is also increasing. The amount of community-created frameworks, libraries, and development tools (called “crates”) is already close to 57k, and more are added every day.

Besides a growing library of tools and frameworks, Rust also has an active and welcoming community. Whether you need help with solving an issue or looking for tips and tricks on using Rust, you have several places to visit. Besides the community chat and user forum, Rust also has an active subreddit section.

Take a look at a few examples of rising community projects:

redox, an operating system written in Rust; 
cgmath, a linear algebra and computer graphics library; 
Iron, a concurrent web framework; 
Doom renderer.

*3. Rust is fast and flexible.*

Rust is considered to be a relatively fast language. It can run considerably faster than Scala especially in performance-critical tasks, when using generic code. There’s a high possibility that in some areas it may run even three times faster than Scala or Java. It’s easy to pick up and use external packages, and Rust’s cargo build tool makes coding simply… simple. 

There are a few factors that make Rust really fast:

It is statically typed and compiled, making it possible to the compiler to optimize the code for speed 
It offers static dispatch of traits: similar to C++ templates, but cleaner
It explicitly tracks ownership of variables. Rust does not assume that any variable with an address can change anytime so optimizations without negatively affecting the code are possible.
It expects variables to be immutable by default (so optimization is easier)
It offers algebraic data types, also pleasant for optimization
It stores data without any overheads, has no runtime or sudden pauses due to lack of garbage collection
It offers zero cost abstraction
Rust may be also considered as a programming language that’s similar to Rust, yet more friendly to optimize and with less painful advanced programming features. 

*4. Rust can be widely used*

If there’s a project where, aside from the importance of performance and low-level optimizations (yet high-level rust functional programming techniques), a safe and stable execution environment is needed, Rust should pass the exam. 

Rust is regarded to be a low-level language, suiting best systems, as well as embedded and other performance critical code. It is believed that it also finds its usage for 3D video games. 

Why is Rust so loved by developers all over the world? First of all, it lets you write code that will most likely never go wrong as the compiler is there to check it all. The problems that are detected in other programming languages in compile-time, do not appear in Rust. It is also good for writing safe time-saving abstractions, and its safety nearly eliminates the need to use immutability. 

Rust is also regarded to be a language used for emerging, innovative niches that care about quality of a mix of performance, speed and safety. 

Since the proof is in the pudding: Rust is a popular programming language for cryptocurrencies and blockchain. It’s a popular choice since it’s easy to understand and learn as well as provides a unique combination of performance and security – and the latter is something that developers are looking for. Rust also delivers tools for those developers to start shipping their code way quicker. And choosing Rust, chances are that cryptocurrency will unlikely crash and be more secure than when using another programming language. Here you can find a list of cryptocurrencies using Rust. 

*5. Several major companies use Rust*
Despite being a relatively young language, Rust is already acknowledged by developers as a step in the right way when it comes to increasing security and ease of use in programming. But not only developers look at Rust with interest – companies, especially the major ones, also switched already or plan to switch to Rust. During AllThingsOpen virtual conference that took place in May, Ryan Levick (Microsoft cloud developer advocate) explained that Rust as a language is “the industry’s best chance for addressing several issues head-on.” While Microsoft does not plan to stop writing in C++ anytime soon, many of its infrastructures are slowly moved to Rust. 

And Microsoft isn’t the only company that realized the potential benefits of switching to Rust language – among the companies that use Rust language is Dropbox, Sentry, Amazon, and Mozilla. 

*Conclusion*

Looking at all the benefits Rust can offer, it’s no surprise that the system’s popularity is only growing. Rust both solves some of the problems, causing many headaches in the developers’ community while keeping the same level of performance as other, more renowned programming languages. And as both developers and the major players in the IT field recognize the potential Rust language has, it might not be an exaggeration to say Rust will be one day one of the most used programming languages in the modern world.

[Read the original post here](https://scalac.io/blog/5-reasons-why-rust-is-the-future-rust-functional-programming/)