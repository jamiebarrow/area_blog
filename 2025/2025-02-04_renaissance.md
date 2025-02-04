# 2025-02-04 - Renaissance

> The Renaissance is a period of history and a European cultural movement covering the 15th and 16th centuries.
> It marked the transition from the Middle Ages to modernity and was characterized by an effort to revive and surpass the ideas of achievements of classical antiquity.
>
> -- Renaissance, Wikipedia

The above extract from Wikipedia's page on the [Renaissance](https://en.wikipedia.org/wiki/Renaissance) captures in my mind a few important points that we see in software engineering today.

These can be summarized into the below areas:

- Revival of classical ideas: the re-imagining of old concepts
- Explosion of innovation: rapid technological advancements driving progress
- Humanity: the rise of human-centered design, user experience and developer experience
- Interdisciplinary thinking: a cross-pollination of fields yielding new approaches
- Breaking from tradition: the rise of decentralization
- Non-traditional funding: Venture Capitalists, Startup culture, Crowdfunding

## Revival of classical ideas

During the Renaissance philosophers revisited the knowledge of the Greek and Roman eras and built upon it.
The printing press and efforts by scholars to tranlate old texts brought knowledge to more people than before.
Philosophy, ethics, logic and science were more easily shared and evolved.
Scientific advancements challenged and transformed traditional astronomy, medicine and mathematics.

In software development we are seeing old paradigms being revisited with modern technology.

- Functional programming
    - there is a resurgence of functional paradigms that once were seen in older languages sucha as Lisp
    - Kotlin is gaining popularity in the Java ecosystem
    - in newer releases C# has been moving towaards functional idioms such as immutable types, pattern matching and discriminated unions
    - higher order functions and the Redux design pattern have been prominent with React, RxJS etc.

- Artificial Intelligence
    - it isn't new, building on decades old mathematical principles
    - advancements in computational power has driven innovation in this field to realize their potential

- Modularity
    - The Unix philosophy of simplicity and modularity is heavily influencing modern architectures
    - Microservice architectures have been on the rise
    - Interconnected pieces of a system's puzzle has become easier due to standardized approaches to service integration
    - Observability and monitoring of distributed systems has become more important

## Explosion of innovation

Just as the printing press and manufacturing lines influenced society, with software engineering we are seeing rapid evolution:

- cloud computing has changed how applications are deployed and scaled
- AI is transforming development workflows with assistive programming, and automation of tasks such as dependency upgrades (e.g. Renovate bot)
- Low Code and No Code platforms are democratizing software creation
    - Visual Basic 4.0 made an influence on me to become a programmer
    - With the ever increasing connectivity between systems, being able to do systems integration is no longer as hard as it used to be
    - Workflows and simple applications can be built using Power Platform, Canvas Apps, Logic Apps


## Human-Centered Design - rise of UX

The style of painting during the Renaissance emphasized realism and perspective making art seem lifelike.
Products have also shifted focus to bring technology into every day lifes.
People no longer need to login to their computer, wait for a modem to connect before opening their mail client to send-and-receive messages.
No, they just look at their Smart Watch when it buzzes to catch up on their messages.
It no longer requires highly specialized equipment to keep track of your heart-rate, this is built into the same smart watch.

Mobile phones can be used with the sound of your voice, and blind people can add value to their lives by asking
Siri or Google about the news of the day, or ask it to play their favourite songs from their youth on Spotify.

Developer experience is also improving with more powerful tooling, easier to understand failures, and prioritizing
efficiency. Immutable systems are becoming more popular due to their stability and ease of use. Containerization
and automation being a defacto building block in most engineering teams.

## Cross-Pollination of Fields

When we think of the artist da Vinci, we should also think of his achievements as engineering, scientist and inventor.
This blending of fields can be seen in software development today:

- AI meets art, with generative models such as MidJourney and DALL-E
- Software meets biology, with computational biology being a module I studied, and these days bioinformatics and CRISPR simulations are changing the medical field
    - I even had a 3D scan of my mouth made in a matter of minutes by my dentist yesterday with a hand-held scanner
- Finance has always benefitted from technology, however cryptography, blockchain and Smart Contracts are redefining what is possible with transactions and could even remove the need for clearing houses and lower transaction fees

## Breaking from Tradition

The Renaissance impacted society's view on traditional authorities, such as the Church's control over knowledge.
The decentralization of thinking can also be seen in the decentralization of software systems.

- Open Source technology plays a huge role and challenges existing software monopolies
    - It may not be the year of the Linux desktop, but the impact of Linux on the server world as well as Android on the mobile phone world is clear
    - Decentralized technologies such as blockchain aims to reduce reliance on centralized authorities such as banks and corporations
    - Federated communities such as BlueSky and Mastodon are seeing a mass migration away from Twitter/X, Facebook, Threads and Instagram

## Startup Culture

The Renaissance thrived because of wealthy patrons like the Medici famioly funding artists and scientists.
Today there are venture capitalists funding innovative startups, fueling a need for rapid development, innovation and efficiency.

Project management has moved towards the more Lean manufacturing principles and Agile philosophy.
Successful projects using these approaches are those that have actually become agile in execution,
while those that have not changed their approach much apart from on paper have achieved far less successes.

## The Software Renaissance

We are in a software Renaissance. Just as the Renaissance bridged the medieval world and the modern era,
today's software movemenets are transitioning from the rigid, centralized ways to more fluid and democratized
approaches. Combining lessons from the past, interdisciplinary innovation and breaking from tradition.

It marks a period of rediscovery, innovation and transformation.

## Command Line Renaissance

Here is a list of the command line tools you may be familiar with and their modern day successors:

- grep
- ls
- find
- cat
- vim
- git

Here is a list of their modern equivalents

- ripgrep
  - recursively searches directories for a regex pattern
  - respects excluded files and folders listed in the gitignore of a git repository
  - supports many of the same features found in `grep`
  - attempts to default options to the most common use cases
  - Rust programming language
  - 6 to 10 times faster than standard GNU grep (see [Benchmarks](https://github.com/BurntSushi/ripgrep?tab=readme-ov-file#quick-examples-comparing-tools))
  - better supports more modern features, such as Unicode encoding support, and colour highlighting, while remaining performant
  - doesn't try to be fully portable nor POSIX compliant, focuses on Windows, macOS and Linux (which most people use)

- eza
  - modern alternative to ls
  - Rust programming language
  - uses colours and icons to distinguish file types and metadata
  - knows about symbolic links, extended attributes and Git
  - can output human readable relative dates
  - recursing into directories to display them as a tree
  - can display hyperlinks

- fd
  - Rust programming language
  - ignores based on gitignore and hidden directories by default
  - case-insensitive by default, but switches to case-sensitive if uppercase character used
  - uses colour highlighting
  - fast due to parallelized traversal
  - supports executing commands against results
  - much faster than `find`, see [Benchmarks](https://github.com/sharkdp/fd?tab=readme-ov-file#benchmark)

- bat
  - like `cat`, but with wings :)
  - supports syntax highlighting, line-numbers, automatic paging, showing whitespace characters
  - integrates well with the other CLI tools

- fzf
  - similar to VS Code and Jetbrains IDE's when trying to navigate to a file
  - uses "fuzzy" matching algorithm in order to do filtering any kind of list
  - by default will traverse the file system, but can take any output

- neovim
  - predominently Lua programming language
  - fork of vim, with aggresive refactoring to simplify maintanance and improve speed of bug fixes and new features
  - includes scripting engine support
  - features have predominently moved to Lua programming language, with its builtin engine
  - enables extensibility points where plugins can be written in modern programming languages, e.g. C#, Rust, JavaScript)
  - enables more advanced terminal user interfaces
  - huge ecosystem, even distributions of plugins such as [LazyVim](https://www.lazyvim.org/) turning the simple editor into a fully fledged IDE

- lazygit
  - Go programming language
  - terminal user interface (TUI) for more easily using Git from the command line

## Web Tooling Renaissance

- esbuild
  - Go programming language
  - built from scratch to replace existing JavaScript based tooling
  - utilizes the parallelism of Go for performance
  - memory is used efficiently
  - supports modern JavaScript ES6 syntax and TypeScript by default

- rspack
  - Rust programming language
  - Webpack compatible and framework agnostic, builds on classic technologies
  - Fast startup and high performance
  - Hot-Module Reload and other features not yet supported in esbuild
  - https://rspack.dev/

- Deno
  - Rust programming language
  - JavaScript, TypeScript and WebAssembly runtime
  - TypeScript as first class language supported by Deno
  - Improved security model by default
  - ES6 modules by default
  - leverages experience from creator of NodeJS in reimagining the runtime as Deno
  - introduces JSR, a TypeScript first package manager built on top of npm, a superset of npm


