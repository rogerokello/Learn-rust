# Rust Learning Roadmap: Beginner to Expert

**Target Audience**: Complete beginner in Rust, with an interest in web development and practical projects.  
**Assumptions**: 5–10 hours/week, no prior systems programming experience.  
**Goal**: Master Rust from basics to expertise through hands-on projects and community engagement, focusing on web development.  
**Timeline**: ~18–24 months to expertise, adjustable based on pace.

---

## Phase 1: Beginner (0–3 Months) – Rust Fundamentals

**Goal**: Learn Rust’s core syntax, ownership model, and basic programming concepts.  
**Duration**: 8–12 weeks (~5–7 hours/week).  
**Focus**: Build intuition for Rust’s ownership and borrowing system.

### Key Topics
- **Syntax**: Variables, data types (scalars: `i32`, `f64`; compounds: tuples, arrays), functions, control flow (`if`, `loop`, `match`).  
- **Ownership & Borrowing**: Ownership rules, references (`&`), borrowing basics (no lifetimes yet).  
- **Error Handling**: Using `Option`, `Result`, and `panic!`.  
- **Cargo Basics**: Creating projects, running tests, using `cargo build`, `cargo run`, `cargo check`.

### Resources
- **[The Rust Programming Language (The Rust Book)](https://doc.rust-lang.org/book/)**: Read Chapters 1–4 (basics, ownership). Free, interactive, beginner-friendly.  
- **[Rustlings](https://github.com/rust-lang/rustlings)**: Complete exercises 1–30 (intro, variables, functions, ownership). Command-line-based.  
- **[Rust Playground](https://play.rust-lang.org/)**: Browser-based tool to experiment with code snippets.  
- **[Exercism Rust Track](https://exercism.org/tracks/rust)**: Solve 5–10 beginner challenges (e.g., “Hello World,” “Reverse a String”).  
- **[Let’s Get Rusty](https://www.youtube.com/c/LetsGetRusty)** (YouTube): Watch “Rust Crash Course” and ownership videos (~1 hour each).  
- **Community**:  
  - Join [Rust Discord](https://rust-lang.org/community) for real-time Q&A.  
  - Follow `#rustlang` on X for tips and project ideas.  
  - Post questions on [Reddit (r/rust)](https://www.reddit.com/r/rust/).

### Weekly Schedule
- **Monday (2 hours)**: Read one Rust Book chapter (e.g., Chapter 2: Programming a Guessing Game), complete 5 Rustlings exercises.  
- **Wednesday (2 hours)**: Solve 1–2 Exercism challenges, test code in Rust Playground.  
- **Friday (1–2 hours)**: Watch a Let’s Get Rusty video, write a small program (e.g., reverse a string using `&str`).  
- **Sunday (1 hour)**: Review code, ask questions on Rust Discord, check X for `#rustlang` updates.

### Projects
- **CLI To-Do List**: Store tasks in a `Vec<String>`, save to a file using `std::fs`, handle input with `std::io`.  
- **Text-Based Calculator**: Implement basic arithmetic (`+`, `-`, `*`, `/`) using `match` and `Option`.

### Milestones
- Write a program processing user input with `Option` or `Result`.  
- Understand owned (`String`) vs. borrowed (`&str`) values.  
- Build and run a CLI project using `cargo`.

---

## Phase 2: Intermediate (3–9 Months) – Practical Web Applications

**Goal**: Build real-world Rust applications (e.g., web servers) and deepen ownership and concurrency knowledge.  
**Duration**: 4–6 months (~6–8 hours/week).  
**Focus**: Apply Rust to web development and async programming.

### Key Topics
- **Advanced Ownership**: Lifetimes, smart pointers (`Box`, `Rc`).  
- **Concurrency**: Threads (`std::thread`), basic async with `tokio` (`async/await`).  
- **Traits & Generics**: Trait-based polymorphism, generic functions, trait bounds.  
- **Crates**: Use `serde` (JSON serialization), `reqwest` (HTTP requests), `axum` (web framework).  
- **Error Handling**: Custom errors with `thiserror` or `anyhow`.

### Resources
- **[The Rust Book](https://doc.rust-lang.org/book/)**: Read Chapters 5–10 (structs, enums, lifetimes, traits).  
- **[Zero to Production in Rust](https://www.zero2prod.com/)** (Luca Palmieri): Build a REST API (first 3 chapters: setup, endpoints, database).  
- **[Rust by Example](https://doc.rust-lang.org/rust-by-example/)**: Explore lifetimes, traits, threads.  
- **[Exercism Rust Track](https://exercism.org/tracks/rust)**: Solve intermediate challenges (e.g., “Anagram”).  
- **[Let’s Get Rusty](https://www.youtube.com/c/LetsGetRusty)**: Watch videos on async Rust and `tokio`.  
- **Community**:  
  - Engage on [Rust Users Forum](https://users.rust-lang.org/) for project feedback.  
  - Share API projects on X with `#rustlang`.

### Weekly Schedule
- **Monday (2 hours)**: Read Rust Book chapter, complete 3–5 Rustlings exercises (e.g., lifetimes).  
- **Wednesday (2 hours)**: Work on Zero to Production (e.g., API endpoints with `axum`), solve 1 Exercism challenge.  
- **Friday (2 hours)**: Build a Rust project (e.g., web server), watch a `tokio` tutorial.  
- **Sunday (1–2 hours)**: Review code, post questions on Rust Discord or X.

### Projects
- **REST API with Axum**: Implement a task manager with CRUD operations using `axum` and `serde` for JSON.  
- **Web Scraper**: Use `reqwest` and `tokio` to fetch/process web data concurrently (e.g., scrape blog titles).  
- **CSV Parser**: Parse a CSV file using `serde`, handle errors with `thiserror`.

### Milestones
- Build a functional REST API with proper error handling.  
- Use `async/await` in a project (e.g., fetch data with `reqwest`).  
- Write a generic function or implement a trait for a custom struct.

---

## Phase 3: Advanced (9–18 Months) – Systems Programming and Optimization

**Goal**: Master low-level Rust features, optimize performance, and contribute to open-source projects.  
**Duration**: 6–9 months (~6–8 hours/week).  
**Focus**: Dive into systems programming, WebAssembly, and performance optimization.

### Key Topics
- **Unsafe Rust**: Use `unsafe` for low-level operations (e.g., raw pointers).  
- **Systems Programming**: Advanced file I/O, C integration (`bindgen`), WebAssembly (`wasm-bindgen`).  
- **Performance**: Profile with `cargo flamegraph`, optimize memory/CPU usage.  
- **Open-Source**: Contribute to Rust crates or projects.

### Resources
- **[Rust for Rustaceans](https://nostarch.com/rust-rustaceans)** (Jon Gjengset): Study unsafe Rust, performance, idiomatic code.  
- **[Rust in Action](https://www.manning.com/books/rust-in-action)**: Focus on systems programming (e.g., file systems).  
- **[Zero to Production](https://www.zero2prod.com/)**: Complete advanced sections (deployment, testing).  
- **[Embedded Rust Book](https://docs.rust-embedded.org/book/)**: Optional for embedded systems.  
- **Community**:  
  - Contribute to [GitHub Rust projects](https://github.com/rust-lang) (e.g., `tokio`, `serde`, “good first issue” tags).  
  - Attend [RustConf](https://rustconf.com/) or local meetups (check X for `#rustlang` events).

### Weekly Schedule
- **Monday (2 hours)**: Read Rust for Rustaceans, experiment with `unsafe` code.  
- **Wednesday (2 hours)**: Work on a systems project (e.g., file parser), profile with `cargo flamegraph`.  
- **Friday (2 hours)**: Contribute to a Rust crate (e.g., fix a bug), watch a WebAssembly tutorial.  
- **Sunday (1–2 hours)**: Share progress on X, get feedback on Rust Users Forum.

### Projects
- **Simple Key-Value Store**: Build a persistent store using file I/O and `tokio`.  
- **WebAssembly App**: Create a browser-based calculator/game with `wasm-bindgen`.  
- **Open-Source Contribution**: Fix a bug or add a feature to a Rust crate (e.g., `serde` documentation).

### Milestones
- Write safe `unsafe` Rust code for a small project.  
- Deploy a Rust web server to production (e.g., AWS, Heroku).  
- Submit a pull request to a Rust crate on GitHub.

---

## Phase 4: Expert (18–24+ Months) – Specialization and Leadership

**Goal**: Specialize in a Rust domain (e.g., web, embedded, WebAssembly), publish crates, and mentor others.  
**Duration**: Ongoing (~5–7 hours/week).  
**Focus**: Lead in the Rust community and build production-grade systems.

### Key Topics
- **Specialization**: Deep dive into web (`axum`), embedded (`no_std`), or WebAssembly.  
- **Crate Development**: Write, test, publish a crate to Crates.io.  
- **Mentorship**: Answer questions on Rust Discord or Exercism.  
- **Cross-Language Integration**: Use Rust with Python (`PyO3`) or C (`bindgen`).

### Resources
- **[Rust RFCs](https://github.com/rust-lang/rfcs)**: Study language evolution.  
- **[Tokio Docs](https://tokio.rs/)**: Master advanced async patterns.  
- **[WebAssembly Docs](https://webassembly.org/)**: Deepen WASM knowledge.  
- **Community**:  
  - Mentor on [Exercism Rust Track](https://exercism.org/tracks/rust) or Rust Discord.  
  - Write a blog or speak at RustConf, share on X with `#rustlang`.

### Projects
- **Publish a Rust Crate**: Create a utility library (e.g., parsing tool) with tests and docs.  
- **Embedded System**: Develop for Arduino/Raspberry Pi using `no_std`.  
- **High-Performance Server**: Build a production-grade server with `tokio` or `hyper` (e.g., chat server).

### Milestones
- Publish a crate used by others on Crates.io.  
- Mentor a beginner or present a Rust talk (e.g., blog post, RustConf).  
- Build and deploy a production-grade Rust application.

---

## General Tips
- **Daily Practice**: Code 30–60 minutes daily (Rustlings, projects).  
- **Project-Driven**: Focus on web projects (e.g., REST APIs, WebAssembly).  
- **Community**: Share on X (#rustlang), join Rust Discord.  
- **Track Progress**: Maintain a GitHub repo for Rust projects.  
- **Debug Ownership**: Practice small ownership exercises to master the borrow checker.

---

## Sample Weekly Schedule (Full Roadmap)
- **Beginner**: 5–7 hours/week (Rust Book, Rustlings, CLI projects).  
- **Intermediate**: 6–8 hours/week (Zero to Production, REST API, concurrency).  
- **Advanced**: 6–8 hours/week (systems programming, open-source).  
- **Expert**: 5–7 hours/week (specialization, crate development, mentoring).

---
