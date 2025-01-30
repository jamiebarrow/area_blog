# 2025-01-30 - What is Rust, and why should I care?

Firstly, that is an excellent question!
If you searched for Rust, you might come across the computer game named [Rust](https://store.steampowered.com/app/252490/Rust/) in which the goal is survival.
While the game is not what this article is about, the goal of surviving in the ever changing software engineering world is still relevant.

[Rust](https://www.rust-lang.org/) is a programming language built with two main objectives:

- Security
- Performance

The first Git commit for the project was on [16 June 2010](c01efc669f09508b55eced32d3c88702578a7c3e) but it dates also to at least [4 years prior](https://github.com/rust-lang/rust/commit/c01efc669f09508b55eced32d3c88702578a7c3e#commitcomment-13619994) where Graydon Hoare worked on it as " a personal project between 2006-2009 and, after late 2009, a Mozilla project conducted in private" - see [rust-prehistory](https://github.com/graydon/rust-prehistory).

So in reality, it isn't actually _that_ new to the software world.

Mozilla are the company known for the browsers wars between Microsoft and Netscape, where the Netscape Communicator browser got open sourced as Mozilla which later became Firefox.

Before Google Chrome, Firefox was the browser that I used day-to-day as a student and as a software developer.
In the old days of web development, there was no "Development Tools" to make things easier to debug. Firefox changed all that by having a browser which was easy to extend.
The Firebug extension is in my eyes the tool that would inspire the evolution of web development tools which we today take for granted as built-in to most modern browsers.

Netscape was also known for the ECMA-262 standard introduced back in 1997, a scripting language developed for the Netscape 2 browser and invented by Brendan Eich.
That is known today as JavaScript, and I believe there's no doubt how it has shaped the more dynamic and interactive internet that we use today.

Except JavaScript is also not perfect.
Many developers joke about how certain things are unintuitive, weird or just plain buggy.
Single page applications that are draining the memory of the computer, nevermind the download size of some websites because of all the various scripts on the pages.
At least these days it is mostly built on a standard base.
Browser incompatibility issues are not as common as the infamous Internet Explorer 6 days.

So why would Mozilla invest in a new programming language when JavaScript was already active and popular?

Even Graydon Hoare, the inventor of Rust, was not so certain about it at the beginning.
He spent many years iterating on his designs and ideas, until he felt it was actually feasible to make his vision become a reality.
Before he even wanted to show it to to anyone else.

Rust was designed to be a systems programming language that runs [blazingly fast](https://prev.rust-lang.org/en-US/), prevents segmentation faults and guarantees thread safety.
The goal of the project was to design and implement a safe, concurrent, practical systems programming language - see [here](https://prev.rust-lang.org/en-US/faq.html).

Interestingly enough they state this as a [non-goal](https://prev.rust-lang.org/en-US/faq.html#what-are-some-non-goals) of Rust:

> 1. We do not employ any particularly cutting-edge technologies. Old, established techniques are better.

I find this ironic, as Rust is in my opinion being seen as a cutting-edge technology, in how it changes the paradigm of how we program traditionally.
What is also interesting is how they state:

> 4. We do not intend to be 100% static, 100% safe, 100% reflective, or too dogmatic in any other sense. Trade-offs exist.

I find these two specific points interesting, because many new technologies arise from a desire to make things better.
However, often these projects come in the form of a re-write, or use of cutting-edge tech, which only leads to high expectations but less impressive results.

I find it interesting because it seems like a mature approach, where the mistakes of the past are not forgotten, and the team wishes to look on legacy just as that:
legacy. Established techniques are proven. There is no such thing as being 100% perfect in the real world.

The goal is not to replace everything that currently exists, but only to target a specific problem set where systems programming is most interested in:

- performance (memory use, concurrent execution, efficiency)
- security (memory safety)
- reliable

It is now 2025, and while it took a long time for inertia, I believe there has been an increase in the buzz of Rust.

It has begun to reach its goals.

Review the below:

- https://leerob.com/n/rust
