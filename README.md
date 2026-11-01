
# Awesome Rust [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
<p align="center">
  <img src="images/awesome-rust.svg" alt="Awesome Rust Logo" width="180">
</p>

Rust is a language empowering everyone to build reliable and efficient software. This repository brings together useful projects, tools, and learning resources from across the Rust ecosystem.  
Whether you are building web applications, working with systems programming, exploring artificial intelligence, or developing embedded software, this list aims to help you find the right tools for your needs.
> Inspired by [awesome-python](https://github.com/vinta/awesome-python).
## Official Links
- [Rust Official Website](https://www.rust-lang.org/)
- [Rust Official Documentation](https://rust-lang.org/learn)
- [Rust Official Github](https://github.com/rust-lang)



## Contents

- [AI & Machine Learning](#ai--machine-learning)
  - [AI Agents](#ai-agents)
  - [AI & Machine Learning Libraries](#ai--machine-learning-libraries)
  - [AI Development Tools & Workflows](#ai-development-tools--workflows)
  - [Model Context Protocol (MCP)](#model-context-protocol-mcp)

- [Web Development](#web-development)
  - [Web Frameworks](#web-frameworks)
  - [Web APIs](#web-apis)
  - [Web Servers](#web-servers)
  - [GraphQL](#graphql)
  - [WebSocket](#websocket)
  - [Authentication](#authentication)
  - [Template Engines](#template-engines)

- [Networking & Communication](#networking--communication)
  - [HTTP Clients](#http-clients)
  - [Networking](#networking)
  - [gRPC](#grpc)
  - [Messaging](#messaging)
  - [Email](#email)
  - [Web Scraping](#web-scraping)

- [Database & Storage](#database--storage)
  - [ORM](#orm)
  - [Database Drivers](#database-drivers)
  - [SQL Databases](#sql-databases)
  - [NoSQL Databases](#nosql-databases)
  - [Caching](#caching)
  - [Search](#search)
  - [Serialization](#serialization)

- [Data & Science](#data--science)
  - [Data Analysis](#data-analysis)
  - [Data Processing & ETL](#data-processing--etl)
  - [Data Visualization](#data-visualization)
  - [Scientific Computing](#scientific-computing)
  - [Geospatial](#geospatial)

- [Developer Tools](#developer-tools)
  - [Testing](#testing)
  - [Debugging](#debugging)
  - [Code Analysis](#code-analysis)
  - [Documentation](#documentation)
  - [Profiling](#profiling)
  - [Algorithms](#algorithms)
  - [Package Managers](#package-managers)
  - [Bundlers](#bundlers)

- [DevOps & Cloud](#devops--cloud)
  - [Cloud](#cloud)
  - [Containers](#containers)
  - [CI/CD](#cicd)
  - [Distributed Systems](#distributed-systems)
  - [Observability & Logging](#observability--logging)

- [CLI & GUI](#cli--gui)
  - [CLI Frameworks](#cli-frameworks)
  - [Terminal UI](#terminal-ui)
  - [GUI Frameworks](#gui-frameworks)
  - [Desktop Applications](#desktop-applications)

- [Media & Graphics](#media--graphics)
  - [Image Processing](#image-processing)
  - [Audio](#audio)
  - [Video](#video)
  - [Graphics & Rendering](#graphics--rendering)
  - [Game Development](#game-development)

- [Rust Language](#rust-language)
  - [Async](#async)
  - [Concurrency](#concurrency)
  - [Macros](#macros)
  - [Rust Memory Management](#rust-memory-management)
  - [Functional Programming](#functional-programming)
  - [FFI](#ffi)
  - [Unsafe Rust](#unsafe-rust)

- [Rust Toolchain](#rust-toolchain)
  - [Cargo](#cargo)
  - [Compilers](#compilers)
  - [Package Management](#package-management)
  - [Linting & Formatting](#linting--formatting)
  - [Build Tools](#build-tools)

- [Embedded & Hardware](#embedded--hardware)
  - [Embedded Systems & Microcontrollers](#embedded-systems--microcontrollers)
  - [Robotics](#robotics)

- [Security](#security)
  - [Cryptography](#cryptography)
  - [TLS](#tls)
  - [Security Auditing](#security-auditing)
  - [Penetration Testing](#penetration-testing)

- [Operating Systems & Systems Programming](#operating-systems--systems-programming)
  - [Operating Systems](#operating-systems)
  - [Filesystems](#filesystems)
  - [System Memory Management](#system-memory-management)
  - [Kernel Development](#kernel-development)
  - [Virtualization](#virtualization)

- [Resources](#resources)
  - [Books](#books)
  - [Courses](#courses)
  - [Tutorials](#tutorials)
  - [Conferences](#conferences)
  - [Communities](#communities)
  - [Podcasts](#podcasts)
  - [Newsletters](#newsletters)

- [Contributing](#contributing)
- [License](#license)

## AI & Machine Learning

Frameworks, libraries, and tools for building AI applications, machine learning systems, and AI-assisted development workflows with Rust.

### AI Agents

- [Rig](https://github.com/0xPlaygrounds/rig)
  - A modular Rust framework for building LLM applications and AI agents with tool calling, multi-turn conversations, streaming, and memory management.
- [LangChain Rust](https://github.com/Abraxas-365/langchain-rust)
  - A Rust implementation of LangChain that provides tool-using agents, memory, LLM chains, and integrations with multiple model providers.
- [OpenAI Codex CLI](https://github.com/openai/codex)
  - An open-source coding agent that runs in the terminal and can read, modify, and execute code.
- [Goose](https://github.com/block/goose)
  - An extensible AI agent built in Rust that can execute commands, edit files, and automate development workflows.
- [OpenHuman](https://github.com/tinyhumansai/openhuman)
  - Open-source Rust based AI agent harness with multi-agent orchestration, persistent memory, and workflow automation.

### AI & Machine Learning Libraries

- [mistral.rs](https://github.com/EricLBuehler/mistral.rs)
  - A fast and flexible Rust inference engine for running quantized large language models locally, with CPU, Apple Silicon, and CUDA support.
- [Candle](https://github.com/huggingface/candle)
  - A minimalist machine learning framework for Rust, with support for running transformer-based language models on CPU and GPU.
- [Burn](https://github.com/tracel-ai/burn)
  - A flexible and portable deep learning framework written in Rust, supporting neural networks, automatic differentiation, model training, and multiple hardware backends.
- [Linfa](https://github.com/rust-ml/linfa)
  - A Rust machine learning toolkit inspired by scikit-learn, providing classical algorithms, preprocessing, clustering, regression, and dimensionality reduction.
- [Neuronika](https://github.com/neuronika/neuronika)
  - A pure Rust deep learning library for building dynamic neural networks with reverse-mode automatic differentiation.
- [tch-rs](https://github.com/LaurentMazare/tch-rs)
  - Rust bindings for the PyTorch C++ API, providing tensor operations, automatic differentiation, neural network modules, and GPU acceleration.
- [Hugging Face Tokenizers](https://github.com/huggingface/tokenizers)
  - A fast and versatile tokenizer library written in Rust, supporting widely used subword tokenization algorithms and pretrained tokenizer models.
- [Lingua](https://github.com/pemistahl/lingua-rs)
  - A language detection library for Rust designed to identify languages accurately, including short text and individual words, with offline support.
- [OpenCV Rust](https://github.com/twistedfall/opencv-rust)
  - Rust bindings for OpenCV, providing access to image processing, object detection, feature extraction, camera calibration, and computer vision algorithms.

### AI Development Tools & Workflows

- [OpenAgents Control](https://github.com/darrenhinde/OpenAgentsControl)
  - A framework for creating repeatable AI coding workflows with reusable patterns, specialized agents, and human approval gates.
- [CC Switch](https://github.com/farion1231/cc-switch)
  - A desktop tool for managing configurations and switching between AI coding assistants and model providers.
- [Agent Desktop](https://github.com/vercel-labs/agent-desktop)
  - A Rust-based computer-use tool that enables AI agents to inspect and operate desktop applications through accessibility APIs.
- [Cloudroom](https://github.com/davidondrej/cloudroom)
  - An open-source desktop platform for managing AI coding agents locally and in the cloud, powered by a Rust-based cloud engine.
- [ai-memory](https://github.com/akitaonrails/ai-memory)
  - Long-term memory and cross-agent handoffs for AI coding agents.
- [Codync](https://github.com/leepokai/Codync)
  - Open-source platform for managing and orchestrating multiple AI coding agents across devices.

### Model Context Protocol (MCP)

- [Official Rust MCP SDK](https://github.com/modelcontextprotocol/rust-sdk)
  - The official Rust SDK for implementing Model Context Protocol clients and servers with asynchronous support.
- [Agent Gateway](https://github.com/agentgateway/agentgateway)
  - A Rust-based gateway for managing and securing connections between AI agents, MCP servers, and model providers.

**[⬆ Back to Top](#contents)**

## Web Development

Frameworks and libraries for building web applications, APIs, and web services.

### Web Frameworks

- [Actix Web](https://github.com/actix/actix-web)
  - A powerful and pragmatic web framework for building web applications.
- [Axum](https://github.com/tokio-rs/axum)
  - An ergonomic and modular web framework built around Tokio and Tower.
- [Rocket](https://github.com/rwf2/Rocket)
  - A web framework focused on usability, security, and developer experience.
- [Poem](https://github.com/poem-web/poem)
  - A full-featured and easy-to-use web framework with flexible routing, middleware, and OpenAPI support.
- [Salvo](https://github.com/salvo-rs/salvo)
  - A powerful and easy-to-use web framework with built-in support for HTTP/2, HTTP/3, OpenAPI, and middleware.
- [Loco](https://github.com/loco-rs/loco)
  - A Rails-inspired full-stack web framework for building web applications and APIs with built-in ORM, authentication, and background jobs.
- [Topcoat](https://github.com/tokio-rs/topcoat)
  - A modular, batteries-included full-stack Rust framework for server-rendered web applications with reactive client-side interactivity.
- [Yew](https://github.com/yewstack/yew)
  - A Rust framework for building client-side web applications using WebAssembly and a component-based architecture.
- [Leptos](https://github.com/leptos-rs/leptos)
  - A full-stack Rust web framework supporting reactive user interfaces, server-side rendering, and WebAssembly.

### Web APIs

- [Utoipa](https://github.com/juhaku/utoipa)
  - A code-first library for automatically generating OpenAPI documentation for Rust REST APIs, with integrations for Axum, Actix Web, and Rocket.
- [Poem OpenAPI](https://github.com/poem-web/poem/tree/master/poem-openapi)
  - A type-safe OpenAPI implementation for the Poem web framework, with support for automatic API documentation and interactive documentation interfaces.

### Web Servers

- [Hyper](https://github.com/hyperium/hyper)
  - HTTP implementation for Rust, used to build HTTP clients and servers.
- [Pingora](https://github.com/cloudflare/pingora)
  - Framework for building HTTP proxies and other network services, developed by Cloudflare.
- [Static Web Server](https://github.com/static-web-server/static-web-server)
  - Serves static files over HTTP and HTTPS, with support for compression, caching, and access control.

### GraphQL

- [async-graphql](https://github.com/async-graphql/async-graphql)
  - GraphQL server library with async support, subscriptions, and integrations for Axum, Poem, and Actix Web.
- [Juniper](https://github.com/graphql-rust/juniper)
  - GraphQL server library that lets you define schemas using Rust types and connect them to existing web frameworks.
- [graphql-client](https://github.com/graphql-rust/graphql-client)
  - Generates type-safe Rust code for GraphQL queries and responses from your schema and query files.

### WebSocket

- [Tokio Tungstenite](https://github.com/snapview/tokio-tungstenite)
  - Asynchronous WebSocket implementation for Tokio, with support for both clients and servers.
- [Fastwebsockets](https://github.com/denoland/fastwebsockets)
  - WebSocket protocol implementation with direct access to frames and support for building clients and servers.

### Authentication

- [axum-login](https://github.com/maxcountryman/axum-login)
  - Handles user authentication and authorization in Axum applications, with support for custom user types and authentication backends.

### Template Engines

- [Askama](https://github.com/askama-rs/askama)
  - Jinja-style templates compiled into Rust code, with template errors checked at compile time.
- [Tera](https://github.com/Keats/tera)
  - Template engine inspired by Jinja2 and Django, with support for template inheritance and data rendering.
- [MiniJinja](https://github.com/mitsuhiko/minijinja)
  - Lightweight Jinja2-style template engine for rendering HTML, configuration files, and other text.
- [Maud](https://github.com/lambda-fairy/maud)
  - HTML templates written directly in Rust using macros, without separate template files.
- [Handlebars](https://github.com/sunng87/handlebars-rust)
  - Rust implementation of Handlebars with support for helpers, partials, and template inheritance.

**[⬆ Back to Top](#contents)**

## Networking & Communication

Libraries and tools for network communication, protocols, and distributed messaging.

### HTTP Clients

- [Reqwest](https://github.com/seanmonstar/reqwest)
  - HTTP client with async and blocking APIs, supporting JSON, multipart requests, cookies, proxies, and TLS.
- [Ureq](https://github.com/algesten/ureq)
  - Synchronous HTTP client for applications that don't need an async runtime.
- [Wreq](https://github.com/0x676e67/wreq)
  - HTTP client with customizable TLS and HTTP/2 settings, proxy support, and browser fingerprint matching.

### Networking

- [rust-libp2p](https://github.com/libp2p/rust-libp2p)
  - Framework for building peer-to-peer applications, with support for peer discovery, connections, and decentralized communication.
- [Iroh](https://github.com/n0-computer/iroh)
  - Library for building direct connections between devices, including connections across NATs.
- [smoltcp](https://github.com/smoltcp-rs/smoltcp)
  - TCP/IP stack designed for embedded and bare-metal systems, with no heap allocation required.
- [Quinn](https://github.com/quinn-rs/quinn)
  - Async implementation of the QUIC protocol for building network clients and servers in Rust.

### gRPC

- [Tonic](https://github.com/grpc/grpc-rust)
  - gRPC implementation for Rust with async/await, HTTP/2, streaming, and Protocol Buffers support.
- [Volo](https://github.com/cloudwego/volo)
  - Rust RPC framework with support for gRPC and Thrift, including code generation from Protocol Buffers.

### Messaging

- [async-nats](https://github.com/nats-io/nats.rs)
  - Rust client for NATS, with support for publish/subscribe, request/reply, JetStream, and key-value storage.
- [Lapin](https://github.com/amqp-rs/lapin)
  - Async AMQP 0-9-1 client for RabbitMQ, supporting message publishing, consuming, and acknowledgements.
- [Apache Iggy](https://github.com/apache/iggy)
  - Persistent message streaming platform with support for streams, topics, partitions, producers, and consumers.
- [RMQTT](https://github.com/rmqtt/rmqtt)
  - MQTT broker for IoT messaging, supporting MQTT 3.1.1 and 5.0, clustering, WebSockets, and TLS.

### Email

- [Lettre](https://github.com/lettre/lettre)
  - Email library for building and sending messages over SMTP, with support for TLS, attachments, and async transports.
- [MailCrab](https://github.com/tweedegolf/mailcrab)
  - Local SMTP server for testing outgoing emails, with a web interface for viewing messages and attachments.

### Web Scraping

- [Spider](https://github.com/spider-rs/spider)
  - Web crawler for collecting pages and links, with support for concurrent crawling and JavaScript-rendered content.
- [Scraper](https://github.com/rust-scraper/scraper)
  - HTML parsing library with CSS selector support for extracting elements and data from web pages.
- [Fantoccini](https://github.com/jonhoo/fantoccini)
  - Async WebDriver client for controlling browsers and interacting with web pages through CSS selectors.

**[⬆ Back to Top](#contents)**

## Database & Storage

Libraries and tools for database connectivity, data persistence, and storage management.

### ORM

- [Diesel](https://github.com/diesel-rs/diesel)
  - ORM and query builder that uses Rust's type system to check database schemas and queries at compile time. Supports PostgreSQL, MySQL, and SQLite.
- [SeaORM](https://github.com/SeaQL/sea-orm)
  - Async ORM for relational databases, with support for entity relationships, migrations, PostgreSQL, MySQL, and SQLite.
- [RBatis](https://github.com/rbatis/rbatis)
  - Async ORM with dynamic SQL, macros, and support for multiple database backends.

### Database Drivers

- [Tokio Postgres](https://github.com/rust-postgres/rust-postgres)
  - Async PostgreSQL driver for Tokio, with support for transactions, prepared statements, and pipelining.
- [Rusqlite](https://github.com/rusqlite/rusqlite)
  - SQLite bindings for Rust, providing an API for executing SQL queries and managing transactions.
- [MongoDB Rust Driver](https://github.com/mongodb/mongo-rust-driver)
  - Official MongoDB driver for Rust, supporting CRUD operations, aggregation, transactions, and change streams.
- [Redis-rs](https://github.com/redis-rs/redis-rs)
  - Redis client for Rust, with support for async and sync connections, Pub/Sub, and pipelining.

### SQL Databases

- [Turso](https://github.com/tursodatabase/turso)
  - SQLite-compatible SQL database written in Rust that runs directly inside an application.
- [SurrealDB](https://github.com/surrealdb/surrealdb)
  - Multi-model database combining relational, document, and graph data with its own query language, SurrealQL.
- [GreptimeDB](https://github.com/GreptimeTeam/greptimedb)
  - Database for storing and querying time series, metrics, logs, and traces using SQL and PromQL.
- [RisingWave](https://github.com/risingwavelabs/risingwave)
  - Streaming database that continuously runs SQL queries on incoming data from sources such as Kafka.
- [Databend](https://github.com/datafuselabs/databend)
  - Cloud-native SQL data warehouse for analytics on large datasets stored in object storage.
- [GlueSQL](https://github.com/gluesql/gluesql)
  - Extensible SQL database engine that works with different storage backends, including memory and files.

### NoSQL Databases

- [TiKV](https://github.com/tikv/tikv)
  - Distributed key-value database with ACID transactions and Raft-based replication.
- [Qdrant](https://github.com/qdrant/qdrant)
  - Vector database for storing and searching embeddings with metadata filtering.
- [Fjall](https://github.com/fjall-rs/fjall)
  - Embedded key-value storage engine based on an LSM-tree, designed for use directly in Rust applications.
- [redb](https://github.com/cberner/redb)
  - Embedded key-value database written in pure Rust with ACID transactions and concurrent readers.

### Caching

- [Moka](https://github.com/moka-rs/moka)
  - Concurrent in-memory cache for synchronous and asynchronous applications, with TTL, TTI, and eviction policies.
- [Foyer](https://github.com/foyer-rs/foyer)
  - Hybrid cache that combines memory and disk storage with asynchronous access.
- [cached](https://github.com/jaemk/cached)
  - Caching library with reusable cache structures and macros for function memoization.

### Search

- [Tantivy](https://github.com/quickwit-oss/tantivy)
  - Rust library for full-text search, inspired by Apache Lucene.
- [Meilisearch](https://github.com/meilisearch/meilisearch)
  - Search engine for applications with typo tolerance and relevant search results.
- [Quickwit](https://github.com/quickwit-oss/quickwit)
  - Distributed search engine for logs, traces, and large-scale event data.
- [Sonic](https://github.com/valeriansaliou/sonic)
  - Lightweight search backend that indexes words and returns document identifiers, with typo correction and autocomplete.
- [ParadeDB](https://github.com/paradedb/paradedb)
  - PostgreSQL extension that adds full-text search, BM25 ranking, and vector search.

### Serialization

- [Serde](https://github.com/serde-rs/serde)
  - Framework for serializing and deserializing Rust data structures across different data formats.
- [Serde JSON](https://github.com/serde-rs/json)
  - JSON support for Serde, with serialization and deserialization of Rust data structures.
- [rkyv](https://github.com/rkyv/rkyv)
  - Zero-copy serialization framework that allows serialized data to be accessed without fully deserializing it.
- [Postcard](https://github.com/jamesmunns/postcard)
  - Compact binary serialization format built on Serde, designed for no_std and embedded systems.
- [simd-json](https://github.com/simd-lite/simd-json)
  - SIMD-based JSON parser for Rust with Serde compatibility.
- [Prost](https://github.com/tokio-rs/prost)
  - Protocol Buffers implementation that generates Rust types from .proto files.
- [RON](https://github.com/ron-rs/ron)
  - Human-readable serialization format with a syntax similar to Rust, built on Serde.

**[⬆ Back to Top](#contents)**

## Data & Science

Libraries for data processing, scientific computing, and analytical applications.

### Data Analysis

- [Polars](https://github.com/pola-rs/polars)
  - DataFrame library for working with structured data, with support for lazy queries, SQL, and parallel processing.
- [Apache DataFusion](https://github.com/apache/datafusion)
  - Extensible SQL query engine built on Apache Arrow for analytical queries over different data sources.
- [Daft](https://github.com/Eventual-Inc/Daft)
  - DataFrame and query engine for processing large datasets, including images, videos, and other multimodal data.

### Data Processing & ETL

- [Apache Arrow Rust](https://github.com/apache/arrow-rs)
  - Rust implementation of Apache Arrow and Parquet for columnar data processing and storage.
- [Delta-rs](https://github.com/delta-io/delta-rs)
  - Rust library for reading and managing Delta Lake tables, including data updates and version history.
- [Apache Iceberg Rust](https://github.com/apache/iceberg-rust)
  - Rust implementation of Apache Iceberg for managing analytical tables, schema evolution, and snapshots.
- [Timely Dataflow](https://github.com/TimelyDataflow/timely-dataflow)
  - Framework for building parallel and distributed dataflow computations.
- [Differential Dataflow](https://github.com/TimelyDataflow/differential-dataflow)
  - Incremental data processing framework that updates computation results as input data changes.
- [Apache SeaTunnel](https://github.com/apache/seatunnel)
  - Data integration platform for moving data between different systems, supporting batch processing, streaming, and CDC.

### Data Visualization

- [Plotly.rs](https://github.com/plotly/plotly.rs)
  - Rust library for creating interactive charts and plots powered by Plotly.js.
- [Rerun](https://github.com/rerun-io/rerun)
  - Visualization tool for exploring multimodal data, including images, point clouds, spatial data, and sensor streams.

### Scientific Computing

- [Faer](https://github.com/sarah-quinones/faer-rs)
  - High-performance linear algebra library for dense and sparse matrices, including matrix decompositions.
- [nalgebra](https://github.com/dimforge/nalgebra)
  - Linear algebra library for vectors, matrices, and geometric transformations.
- [ndarray](https://github.com/rust-ndarray/ndarray)
  - N-dimensional array library with slicing, array views, and numerical operations.

### Geospatial

- [Geo](https://github.com/georust/geo)
  - Geospatial library for points, lines, polygons, geometric operations, and distance calculations.

**[⬆ Back to Top](#contents)**

## Developer Tools

Tools and libraries that improve the software development workflow.

### Testing

- [Nextest](https://github.com/nextest-rs/nextest)
  - A test runner for Rust with parallel execution, test filtering, retries, and CI reporting.
- [Insta](https://github.com/mitsuhiko/insta)
  - Snapshot testing library for comparing test output against saved reference snapshots.
- [Proptest](https://github.com/proptest-rs/proptest)
  - Property-based testing library that generates random inputs to test program behavior.
- [rstest](https://github.com/la10736/rstest)
  - Fixture-based testing framework with parameterized tests and reusable test setup.
- [Mockall](https://github.com/asomers/mockall)
  - Mock object library for creating test doubles from Rust traits and structs.
- [cargo-llvm-cov](https://github.com/taiki-e/cargo-llvm-cov)
  - Cargo subcommand for measuring Rust code coverage using LLVM instrumentation.
- [Testcontainers](https://github.com/testcontainers/testcontainers-rs)
  - Runs temporary containers such as databases and services for integration tests.
- [test-log](https://github.com/d-e-s-o/test-log)
  - Test attribute that initializes logging or tracing before running tests.
- [cargo-fuzz](https://github.com/rust-fuzz/cargo-fuzz)
  - Cargo subcommand for fuzz testing Rust code with libFuzzer.

### Debugging

- [Tokio Console](https://github.com/tokio-rs/console)
  - Interactive debugging tool for monitoring Tokio tasks, async operations, and runtime resources.
- [Tracing](https://github.com/tokio-rs/tracing)
  - Instrumentation framework for collecting structured events and diagnostic information from Rust applications.
- [Ey​​re](https://github.com/eyre-rs/eyre)
  - Error reporting library with customizable error reports and backtrace support.
- [Backtrace](https://github.com/rust-lang/backtrace-rs)
  - Library for capturing stack traces and resolving function names and source locations at runtime.
- [addr2line](https://github.com/gimli-rs/addr2line)
  - Resolves executable addresses into function names, source files, line numbers, and stack frames using DWARF debug information.
- [gimli](https://github.com/gimli-rs/gimli)
  - Library for reading and writing DWARF debugging information used by debuggers and other development tools.

### Code Analysis

- [Clippy](https://github.com/rust-lang/rust-clippy)
  - A collection of Rust lints that detects common mistakes, suspicious code, and performance issues.
- [cargo-deny](https://github.com/EmbarkStudios/cargo-deny)
  - Checks project dependencies for license compliance, security advisories, duplicate versions, and allowed sources.
- [cargo-udeps](https://github.com/est31/cargo-udeps)
  - Finds unused dependencies in Cargo projects.
- [cargo-machete](https://github.com/bnjbvr/cargo-machete)
  - Detects unused dependencies declared in Cargo.toml files.
- [cargo-semver-checks](https://github.com/obi1kenobi/cargo-semver-checks)
  - Checks whether changes to a Rust library's public API break semantic versioning compatibility.
- [cargo-geiger](https://github.com/geiger-rs/cargo-geiger)
  - Measures the amount of unsafe Rust code in a project and its dependencies.
- [Biome](https://github.com/biomejs/biome)
  - A fast web development toolchain written in Rust, providing a formatter and linter for JavaScript, TypeScript, JSON, CSS, and other web technologies.
- [Ruff](https://github.com/astral-sh/ruff)
  - Extremely fast Python linter and code formatter written in Rust, with hundreds of lint rules and automatic code fixes.
- [ty](https://github.com/astral-sh/ty)
  - Extremely fast Python type checker and language server written in Rust, providing static type analysis and rich diagnostics.

### Documentation

- [mdBook](https://github.com/rust-lang/mdBook)
  - Creates books and documentation websites from Markdown files.
- [cargo-readme](https://github.com/webern/cargo-readme)
  - Generates README.md files from Rust crate documentation comments.
- [cargo-rdme](https://github.com/orium/cargo-rdme)
  - Generates or updates README sections from crate-level Rust documentation comments.
- [document-features](https://github.com/slint-ui/document-features)
  - Generates documentation for Cargo feature flags from comments in Cargo.toml.

### Profiling

- [Samply](https://github.com/mstange/samply)
  - Cross-platform sampling profiler for analyzing CPU usage with the Firefox Profiler interface.
- [Flamegraph](https://github.com/flamegraph-rs/flamegraph)
  - Generates flame graphs from profiling data to visualize CPU time spent in functions.
- [Puffin](https://github.com/EmbarkStudios/puffin)
  - Instrumentation profiler for measuring execution time in functions and code sections.
- [hotpath](https://github.com/hotpath-rs/hotpath)
  - Profiler for CPU, memory allocations, async operations, SQL queries, and HTTP requests.
- [Inferno](https://github.com/jonhoo/inferno)
  - Rust library and command-line tools for generating flame graphs from stack traces and profiling data.
- [profiling](https://github.com/aclysma/profiling)
  - Common profiling API that integrates with backends such as Puffin, Tracy, and Superluminal.

### Algorithms

- [Petgraph](https://github.com/petgraph/petgraph)
  - Graph data structure library with algorithms for shortest paths, minimum spanning trees, graph traversal, and more.
- [Pathfinding](https://github.com/evenfurther/pathfinding)
  - Implements pathfinding, graph traversal, shortest-path, and flow algorithms such as A*, BFS, and Dijkstra.
- [TheAlgorithms/Rust](https://github.com/TheAlgorithms/Rust)
  - Collection of algorithm implementations in Rust, covering sorting, searching, graph algorithms, and data structures.
- [Polyanya](https://github.com/vleue/polyanya)
  - Implements any-angle pathfinding on navigation meshes for finding optimal paths.
- [Condor](https://github.com/bnomei/condor)
  - Pathfinding library with grid search, polygonal pathfinding, navigation meshes, and route planning.

### Package Managers

- [Bun](https://github.com/oven-sh/bun)
  - Fast all-in-one JavaScript and TypeScript toolkit written in Rust, featuring a runtime, bundler, test runner, and package manager.
- [uv](https://github.com/astral-sh/uv)
  - Extremely fast Python package and project manager written in Rust, with dependency management, lockfiles, virtual environments, and Python version management.

### Bundlers

- [Rolldown](https://github.com/rolldown/rolldown)
  - A fast Rust-based JavaScript and TypeScript bundler with a Rollup-compatible API.

**[⬆ Back to Top](#contents)**

## DevOps & Cloud

Tools and libraries for infrastructure, deployment, cloud services, and operations.

### Cloud

- [AWS SDK for Rust](https://github.com/awslabs/aws-sdk-rust)
  - Official Rust SDK for interacting with AWS services.
- [Firecracker](https://github.com/firecracker-microvm/firecracker)
  - Lightweight virtualization technology for running secure microVMs.
- [Spin](https://github.com/spinframework/spin)
  - Framework for building and running WebAssembly applications in the cloud.
- [Bottlerocket](https://github.com/bottlerocket-os/bottlerocket)
  - Linux-based operating system designed for running containers in cloud environments.
- [Vector](https://github.com/vectordotdev/vector)
  - Observability data pipeline for collecting, processing, and routing logs, metrics, and traces.

### Containers

- [youki](https://github.com/youki-dev/youki)
  - OCI-compatible container runtime written in Rust.
- [runwasi](https://github.com/containerd/runwasi)
  - Library for running WebAssembly workloads with containerd.

### CI/CD

- [release-plz](https://github.com/release-plz/release-plz)
  - Automates Rust crate releases, version updates, changelogs, and publishing from CI.
- [cargo-release](https://github.com/crate-ci/cargo-release)
  - Automates crate releases, including versioning, Git tagging, and publishing.
- [cargo-dist](https://github.com/axodotdev/cargo-dist)
  - Automates cross-platform binary builds, installers, and release distribution through CI.
- [git-cliff](https://github.com/orhun/git-cliff)
  - Generates changelogs from Git history and conventional commits.

### Distributed Systems

- [OpenRaft](https://github.com/databendlabs/openraft)
  - Raft consensus implementation for building fault-tolerant distributed systems.
- [raft-rs](https://github.com/tikv/raft-rs)
  - Rust implementation of the Raft consensus algorithm for replicated state machines.

### Observability & Logging

- [OpenTelemetry Rust](https://github.com/open-telemetry/opentelemetry-rust)
  - Instrumentation and telemetry collection for metrics, logs, and traces.
- [metrics](https://github.com/metrics-rs/metrics)
  - Metrics ecosystem for recording counters, gauges, and histograms in Rust applications.
- [log](https://github.com/rust-lang/log)
  - Logging facade providing macros such as `info!`, `warn!`, and `error!`.
- [env_logger](https://github.com/rust-cli/env_logger)
  - Simple logger with log-level filtering through environment variables.
- [log4rs](https://github.com/estk/log4rs)
  - Configurable logging framework with support for multiple outputs and appenders.

**[⬆ Back to Top](#contents)**

## CLI & GUI

Frameworks and libraries for building command-line, terminal-based, and graphical applications.

### CLI Frameworks

- [Clap](https://github.com/clap-rs/clap)
  - Command-line argument parser with support for subcommands, flags, and automatic help generation.
- [Argh](https://github.com/google/argh)
  - Derive-based argument parsing library for building command-line interfaces.
- [Dialoguer](https://github.com/console-rs/dialoguer)
  - Library for creating interactive CLI prompts, selections, and confirmations.
- [Inquire](https://github.com/mikaelmello/inquire)
  - Interactive CLI framework with text input, selections, and multi-selection prompts.

### Terminal UI

- [Ratatui](https://github.com/ratatui/ratatui)
  - Library for building terminal interfaces with widgets, layouts, tables, charts, and custom rendering.
- [Cursive](https://github.com/gyscos/cursive)
  - Framework for building terminal applications with dialogs, menus, forms, and reusable views.
- [TUI Realm](https://github.com/veeso/tui-realm)
  - Component-based framework for building terminal user interfaces with widgets and event handling.
- [TachyonFX](https://github.com/ratatui/tachyonfx)
  - Library for adding animations and visual effects to Ratatui applications.

### GUI Frameworks

- [Iced](https://github.com/iced-rs/iced)
  - Cross-platform GUI framework with a declarative, widget-based approach.
- [egui](https://github.com/emilk/egui)
  - Immediate-mode GUI library for building desktop applications and interactive tools.
- [Slint](https://github.com/slint-ui/slint)
  - Declarative GUI framework for desktop, embedded, and mobile applications.
- [Makepad](https://github.com/makepad/makepad)
  - Framework for building multi-platform user interfaces with GPU rendering.
- [Dioxus](https://github.com/DioxusLabs/dioxus)
  - Component-based framework for building web, desktop, and mobile applications.
- [Freya](https://github.com/marc2332/freya)
  - Declarative GUI framework for building desktop applications with components and styling.
- [Relm4](https://github.com/Relm4/Relm4)
  - Framework for building GTK4 applications in Rust using a component-based architecture.
- [Xilem](https://github.com/linebender/xilem)
  - Data-driven GUI framework for building reactive user interfaces.
- [Tauri](https://github.com/tauri-apps/tauri)
  - Framework for building desktop applications with web frontends and Rust backends.

### Desktop Applications

- [Zed](https://github.com/zed-industries/zed)
  - High-performance code editor with built-in collaboration and AI features.
- [Lapce](https://github.com/lapce/lapce)
  - Fast, open-source code editor built with Rust.
- [RustDesk](https://github.com/rustdesk/rustdesk)
  - Open-source remote desktop application for remote access and support.
- [Pake](https://github.com/tw93/Pake)
  - Tool for packaging websites into lightweight desktop applications.
- [Rnote](https://github.com/flxzt/rnote)
  - Vector-based drawing and note-taking application for handwritten notes and sketches.
- [Kando](https://github.com/kando-menu/kando)
  - Cross-platform pie menu for launching applications and performing actions.

**[⬆ Back to Top](#contents)**

## Media & Graphics

Libraries and tools for multimedia processing, graphics, rendering, and game development.

### Image Processing

- [Image](https://github.com/image-rs/image)
  - Rust library for loading, processing, and saving images in various formats.
- [Photon](https://github.com/silvia-odwyer/photon)
  - Fast image processing library with filters, effects, and transformations.
- [Oxipng](https://github.com/oxipng/oxipng)
  - Multithreaded PNG optimizer that reduces file sizes without losing image quality.
- [dssim](https://github.com/kornelski/dssim)
  - Image similarity comparison tool based on perceptual differences.

### Audio

- [Rodio](https://github.com/RustAudio/rodio)
  - Audio playback library for playing, mixing, and controlling sound.
- [CPAL](https://github.com/RustAudio/cpal)
  - Cross-platform audio I/O library for recording and playback.
- [Symphonia](https://github.com/pdeljanov/Symphonia)
  - Pure Rust multimedia format decoding library with support for common audio formats.
- [Kira](https://github.com/tesselode/kira)
  - Audio library for games with support for sound effects, music, and spatial audio.
- [NIH-plug](https://github.com/robbert-vdh/nih-plug)
  - Framework for developing audio plugins in Rust.
- [Handy](https://github.com/cjpais/Handy)
  - Cross-platform, offline speech-to-text application built with Rust, featuring real-time audio processing and local AI transcription.

### Video

- [Rust FFmpeg](https://github.com/zmwangx/rust-ffmpeg)
  - Rust bindings for the FFmpeg multimedia framework.
- [Av1an](https://github.com/rust-av/Av1an)
  - Video encoding automation tool for AV1 and other codecs.

### Graphics & Rendering

- [Vello](https://github.com/linebender/vello)
  - GPU-accelerated 2D graphics renderer.
- [Kurbo](https://github.com/linebender/kurbo)
  - Library for working with curves and geometric shapes.
- [Tiny Skia](https://github.com/linebender/tiny-skia)
  - Lightweight 2D graphics rendering library.
- [wgpu](https://github.com/gfx-rs/wgpu)
  - Cross-platform graphics API written in Rust.
- [Vulkano](https://github.com/vulkano-rs/vulkano)
  - Safe Rust wrapper for the Vulkan graphics API.
- [three-d](https://github.com/asny/three-d)
  - Cross-platform 2D and 3D rendering library.
- [Pixels](https://github.com/parasyte/pixels)
  - Hardware-accelerated pixel framebuffer renderer.

### Game Development

- [Bevy](https://github.com/bevyengine/bevy)
  - Data-driven game engine built in Rust.
- [Macroquad](https://github.com/not-fl3/macroquad)
  - Cross-platform game engine for 2D and 3D games.
- [Fyrox](https://github.com/FyroxEngine/Fyrox)
  - 2D and 3D game engine written in Rust.
- [ggez](https://github.com/ggez/ggez)
  - Lightweight game development framework for Rust.
- [Rapier](https://github.com/dimforge/rapier)
  - Physics engine for 2D and 3D games.
- [Avian](https://github.com/avianphysics/avian)
  - ECS-driven 2D and 3D physics engine for Bevy.
- [Piston](https://github.com/PistonDevelopers/piston)
  - Modular game engine written in Rust.

**[⬆ Back to Top](#contents)**

## Rust Language

Libraries and resources related to Rust language features and programming paradigms.

### Async

- [Tokio](https://github.com/tokio-rs/tokio)
  - Asynchronous runtime for networking, I/O, timers, and task scheduling.
- [Smol](https://github.com/smol-rs/smol)
  - Small and fast asynchronous runtime for Rust.
- [Futures](https://github.com/rust-lang/futures-rs)
  - Zero-cost abstractions for asynchronous programming.
- [Monoio](https://github.com/monoio-rs/monoio)
  - Asynchronous runtime based on io_uring.
- [Compio](https://github.com/compio-rs/compio)
  - Thread-per-core async runtime with support for IOCP and io_uring.

### Concurrency

- [Rayon](https://github.com/rayon-rs/rayon)
  - Data parallelism library for executing computations across multiple threads.
- [Crossbeam](https://github.com/crossbeam-rs/crossbeam)
  - Tools and primitives for concurrent programming in Rust.
- [Parking Lot](https://github.com/Amanieu/parking_lot)
  - Efficient synchronization primitives for multithreaded applications.
- [Loom](https://github.com/tokio-rs/loom)
  - Concurrency testing tool for exploring possible thread execution orders.
- [Flume](https://github.com/zesterer/flume)
  - Fast and safe multi-producer, multi-consumer channel.

### Macros

- [Syn](https://github.com/dtolnay/syn)
  - Parsing library for Rust source code and procedural macros.
- [Quote](https://github.com/dtolnay/quote)
  - Quasi-quoting library for generating Rust code.
- [Bon](https://github.com/elastio/bon)
  - Builder generator using Rust procedural macros.
- [Async Trait](https://github.com/dtolnay/async-trait)
  - Enables async functions in trait definitions and implementations.
- [Thiserror](https://github.com/dtolnay/thiserror)
  - Derive macros for implementing standard error traits.
- [Inventory](https://github.com/dtolnay/inventory)
  - Typed plugin registration through distributed collections.

### Rust Memory Management

- [Bumpalo](https://github.com/fitzgen/bumpalo)
  - Fast bump allocation arena for Rust.
- [Slotmap](https://github.com/orlp/slotmap)
  - Slot-based storage with stable keys for managing objects.

### Functional Programming

- [Itertools](https://github.com/rust-itertools/itertools)
  - Extra iterator adaptors, methods, functions, and macros for Rust.
- [Num](https://github.com/rust-num/num)
  - Collection of numeric types and traits for Rust.
- [Frunk](https://github.com/lloydmeta/frunk)
  - Functional generic programming library with HLists and type-level abstractions.

### FFI

- [Rust Bindgen](https://github.com/rust-lang/rust-bindgen)
  - Automatically generates Rust FFI bindings to C and C++ libraries.
- [CXX](https://github.com/dtolnay/cxx)
  - Safe interoperability between Rust and C++.
- [Cbindgen](https://github.com/mozilla/cbindgen)
  - Generates C and C++ headers from Rust code.
- [UniFFI](https://github.com/mozilla/uniffi-rs)
  - Generates foreign language bindings for Rust libraries.
- [PyO3](https://github.com/PyO3/pyo3)
  - Rust bindings for the Python interpreter.
- [NAPI-RS](https://github.com/napi-rs/napi-rs)
  - Framework for building Node.js native add-ons in Rust.
- [Wasm-bindgen](https://github.com/wasm-bindgen/wasm-bindgen)
  - Facilitates interactions between WebAssembly and JavaScript.
- [JNI-RS](https://github.com/jni-rs/jni-rs)
  - Rust bindings for the Java Native Interface.

### Unsafe Rust

- [Bytemuck](https://github.com/Lokathor/bytemuck)
  - Utilities for safely converting and working with byte representations.
- [Zerocopy](https://github.com/google/zerocopy)
  - Zero-cost memory manipulation with safe abstractions over unsafe code.
- [Miri](https://github.com/rust-lang/miri)
  - Interpreter for detecting undefined behavior in Rust programs.
- [SmallVec](https://github.com/servo/rust-smallvec)
  - Vector implementation that stores small collections inline on the stack.
- [Libc](https://github.com/rust-lang/libc)
  - Raw bindings to platform-specific C APIs.

**[⬆ Back to Top](#contents)**

## Rust Toolchain

Tools for compiling, building, formatting, and managing Rust projects.

### Cargo

- [cargo-binstall](https://github.com/cargo-bins/cargo-binstall)
  - Installs Rust binaries directly from prebuilt releases instead of compiling them from source.
- [cargo-edit](https://github.com/killercup/cargo-edit)
  - Provides commands for adding, removing, and upgrading dependencies in Cargo.toml.
- [cargo-generate](https://github.com/cargo-generate/cargo-generate)
  - Creates new Rust projects from existing Git repository templates.
- [cargo-expand](https://github.com/dtolnay/cargo-expand)
  - Displays expanded Rust macros and derive implementations for easier inspection.
- [cargo-msrv](https://github.com/foresterre/cargo-msrv)
  - Identifies the minimum Rust version required to compile a crate.

### Compilers

- [Cranelift Codegen Backend](https://github.com/rust-lang/rustc_codegen_cranelift)
  - An alternative Rust compiler backend that uses Cranelift to generate machine code.
- [GCC Codegen Backend](https://github.com/rust-lang/rustc_codegen_gcc)
  - Enables Rust programs to be compiled through GCC as an alternative code generation backend.
- [Rust-GPU](https://github.com/rust-gpu/rust-gpu)
  - Provides a Rust toolchain for compiling GPU shaders to SPIR-V.
- [Gleam](https://github.com/gleam-lang/gleam)
  - A compiler for the Gleam programming language, targeting Erlang and JavaScript.
- [Roc](https://github.com/roc-lang/roc)
  - A compiler for a fast, friendly, and functional programming language.
- [tsrs](https://github.com/oxc-project/tsrs)
  - A Rust implementation of the TypeScript 7 compiler and language server, designed for faster type checking and lower memory usage.
- [SWC](https://github.com/swc-project/swc)
  - A high-performance JavaScript and TypeScript compiler written in Rust, providing fast code transformation and minification.

### Package Management

- [cargo-update](https://github.com/nabijaczleweli/cargo-update)
  - Installs and updates Rust binaries installed through `cargo install`.
- [cargo-sweep](https://github.com/holmgr/cargo-sweep)
  - Removes stale Cargo build artifacts to reclaim disk space.
- [crates.io](https://github.com/rust-lang/crates.io)
  - The official Rust package registry, providing infrastructure for publishing and downloading crates.

### Linting & Formatting

- [Taplo](https://github.com/tamasfe/taplo)
  - Provides formatting, validation, and language-server support for TOML files.

### Build Tools

- [Cross](https://github.com/cross-rs/cross)
  - Simplifies cross-compiling and testing Rust projects for different target platforms using Docker.
- [cargo-zigbuild](https://github.com/rust-cross/cargo-zigbuild)
  - Enables cross-compilation of Rust applications using Zig as a linker.
- [sccache](https://github.com/mozilla/sccache)
  - Caches compiler outputs to accelerate repeated Rust builds and reduce compilation time.
- [cargo-chef](https://github.com/LukeMathWalker/cargo-chef)
  - Optimizes Rust Docker builds by separating dependency compilation from application source changes.

**[⬆ Back to Top](#contents)**

## Embedded & Hardware

Libraries and tools for embedded development and hardware interaction.

### Embedded Systems & Microcontrollers

- [Tock OS](https://github.com/tock/tock)
  - An embedded operating system designed for secure and reliable applications on microcontrollers.
- [RTIC](https://github.com/rtic-rs/rtic)
  - A real-time concurrency framework for building efficient and predictable embedded applications in Rust.
- [Embassy](https://github.com/embassy-rs/embassy)
  - An asynchronous embedded framework providing executor, HAL, networking, and hardware support for microcontrollers.
- [Embedded HAL](https://github.com/rust-embedded/embedded-hal)
  - Provides hardware abstraction traits for building portable embedded drivers and applications.
- [ESP HAL](https://github.com/esp-rs/esp-hal)
  - Hardware abstraction layers for developing embedded applications on Espressif microcontrollers.
- [RP HAL](https://github.com/rp-rs/rp-hal)
  - Hardware abstraction libraries for Raspberry Pi RP2040 and RP2350 microcontrollers.
- [AVR HAL](https://github.com/Rahix/avr-hal)
  - Hardware abstraction libraries and tools for programming AVR microcontrollers in Rust.
- [probe-rs](https://github.com/probe-rs/probe-rs)
  - A toolkit for flashing, debugging, and interacting with ARM, RISC-V, and Xtensa microcontrollers.
- [defmt](https://github.com/knurling-rs/defmt)
  - An efficient logging framework designed for resource-constrained devices and embedded microcontrollers.
- [Cortex-M](https://github.com/rust-embedded/cortex-m)
  - A collection of Rust crates providing peripheral access, CPU intrinsics, startup support, and debugging utilities for Cortex-M microcontrollers.
- [STM32 Peripheral Access Crates](https://github.com/stm32-rs/stm32-rs)
  - Generated peripheral access crates for a wide range of STM32 microcontroller families.

### Robotics

- [Dora](https://github.com/dora-rs/dora)
  - A dataflow framework for building distributed robotic and AI applications with low-latency communication between nodes.
- [Copper](https://github.com/copper-project/copper-rs)
  - A Rust robotics runtime for building, executing, recording, and replaying robot task graphs from Linux to bare-metal systems.
- [microduck](https://github.com/pollen-robotics/microduck)
  - Rust based software stack for a small bipedal robot, featuring real-time motor control, reinforcement learning policies, and hardware management.

**[⬆ Back to Top](#contents)**

## Security

Libraries and tools for application security, cryptography, and secure development.

### Cryptography

- [RustCrypto Hashes](https://github.com/RustCrypto/hashes)
  - A collection of pure Rust implementations of cryptographic hash functions, including SHA-2, SHA-3, and BLAKE2.
- [Curve25519-Dalek](https://github.com/dalek-cryptography/curve25519-dalek)
  - A pure Rust implementation of Curve25519 elliptic curve operations and related cryptographic primitives.
- [Ring](https://github.com/briansmith/ring)
  - A cryptographic library providing primitives for encryption, hashing, digital signatures, and key exchange.
- [BLAKE3](https://github.com/BLAKE3-team/BLAKE3)
  - A high-performance cryptographic hash function supporting parallel processing and incremental hashing.

### TLS

- [Rustls](https://github.com/rustls/rustls)
  - A modern TLS library written entirely in Rust for secure client and server connections.
- [s2n-tls](https://github.com/aws/s2n-tls)
  - A compact and security-focused TLS implementation developed by AWS, with Rust bindings.

### Security Auditing

- [Cargo Audit (RustSec)](https://github.com/RustSec/rustsec)
  - Scans `Cargo.lock` files for dependencies with known security vulnerabilities using the RustSec Advisory Database.
- [Cargo Vet](https://github.com/mozilla/cargo-vet)
  - Helps verify that third-party Rust dependencies have been audited by trusted reviewers.
- [RustSec Advisory Database](https://github.com/RustSec/advisory-db)
  - A database of security advisories affecting Rust packages published on crates.io.

### Penetration Testing

- [RustScan](https://github.com/bee-san/RustScan)
  - Modern, fast port scanner with Nmap integration.
- [feroxbuster](https://github.com/epi052/feroxbuster)
  - Fast, recursive content discovery tool for web applications.
- [sn0int](https://github.com/kpcyrd/sn0int)
  - Semi-automatic OSINT framework for reconnaissance and attack surface enumeration.

**[⬆ Back to Top](#contents)**

## Operating Systems & Systems Programming

Libraries, tools, and projects for low-level programming and operating system development.

### Operating Systems

- [Redox](https://github.com/redox-os/redox)
  - A Unix-like operating system written in Rust, featuring its own kernel, drivers, and system utilities.
- [Asterinas](https://github.com/asterinas/asterinas)
  - A Linux-compatible operating system kernel written in Rust, designed with memory safety and performance in mind.

### Filesystems

- [Fuser](https://github.com/cberner/fuser)
  - Provides a Rust library for implementing userspace filesystems using the FUSE interface.

### System Memory Management

- [Mimalloc Rust](https://github.com/purpleprotocol/mimalloc_rust)
  - Provides Rust bindings for Microsoft's mimalloc memory allocator.

### Kernel Development

- [Rust for Linux](https://github.com/Rust-for-Linux/linux)
  - Adds Rust language support and abstractions for developing Linux kernel components.
- [Bootloader](https://github.com/rust-osdev/bootloader)
  - Provides bootloaders for starting custom operating system kernels written in Rust.

### Virtualization

- [Cloud Hypervisor](https://github.com/cloud-hypervisor/cloud-hypervisor)
  - A modern virtual machine monitor built with Rust, designed for cloud workloads.
- [crosvm](https://github.com/google/crosvm)
  - A secure virtual machine monitor written in Rust, used by ChromeOS.

**[⬆ Back to Top](#contents)**

## Resources

Learning materials and community resources for Rust developers.

### Books

- [Programming Rust](https://www.oreilly.com/library/view/programming-rust-2nd/9781492052586/)
  - A comprehensive guide to systems programming with Rust, covering ownership, concurrency, and performance.
- [Rust for Rustaceans](https://rust-for-rustaceans.com/)
  - An advanced guide to writing idiomatic, efficient, and maintainable Rust code.
- [Zero To Production In Rust](https://www.zero2prod.com/)
  - A practical book on building reliable, production-ready backend applications with Rust.
- [Rust Atomics and Locks](https://marabos.nl/atomics/)
  - Explores concurrent programming in Rust through atomics, memory ordering, and synchronization primitives.

### Courses

- [Comprehensive Rust](https://google.github.io/comprehensive-rust/)
  - A free, comprehensive Rust course developed by Google, covering fundamentals, concurrency, and embedded programming.
- [Exercism – Rust Track](https://exercism.org/tracks/rust)
  - An interactive learning path with coding exercises and optional mentor feedback.
- [JetBrains Academy – Learn Rust](https://academy.jetbrains.com/course/16631)
  - A hands-on beginner course with coding exercises, instant feedback, and a completion certificate.
- [Getting Started with Rust – Linux Foundation](https://training.linuxfoundation.org/express-learning/getting-started-with-rust-lfel1002/)
  - A self-paced introductory course covering Rust syntax, Cargo, troubleshooting, and practical exercises.
- [100 Exercises To Learn Rust](https://rust-exercises.com/)
  - A progressive, exercise-driven course that teaches Rust through practical coding challenges.
- [Brown University – Interactive Rust Book](https://rust-book.cs.brown.edu/)
  - An interactive learning experience with quizzes and visualizations to help understand Rust ownership and borrowing.

### Tutorials

- [Learn Rust](https://learnrust.net/)
  - A beginner-friendly tutorial series covering Rust fundamentals through step-by-step lessons, examples, and quizzes.
- [Rust Tutorial](https://www.rusttutorial.org/)
  - Practical Rust lessons with runnable examples and guided projects, from basic syntax to async programming.
- [Buzzard – Learn Rust by Example](https://buzzard.clivern.com/)
  - A hands-on tutorial with 60 lessons covering Rust fundamentals, ownership, borrowing, and advanced concepts.
- [Crust of Rust](https://www.youtube.com/playlist?list=PLqbS7AVVErFiWDOAVrPt7aYmnuuOLYvOa)
  - An in-depth video series by Jon Gjengset exploring advanced Rust concepts through live coding.
- [Hecto: Build Your Own Text Editor in Rust](https://flenker.blog/hecto/)
  - A step-by-step tutorial on building a terminal text editor from scratch using Rust.
- [Writing an OS in Rust](https://os.phil-opp.com/)
  - A practical tutorial series on building an operating system kernel with Rust.
- [Game Development with Macroquad](https://mq.agical.se/)
  - A project-based guide to creating 2D games with Rust and the Macroquad game framework.
- [Build a Lua Interpreter in Rust](https://wubingzheng.github.io/build-lua-in-rust/en/)
  - A tutorial series that teaches interpreter development by implementing Lua in Rust.

### Conferences

- [RustConf](https://rustconf.com/)
  - The flagship annual Rust conference bringing together developers, maintainers, and researchers from across the Rust ecosystem.
- [RustWeek](https://rustweek.org/)
  - A week-long Rust community event featuring technical talks, workshops, hackathons, and networking.
- [Oxidize](https://oxidizeconf.com/)
  - A conference focused on practical Rust adoption, production engineering, and real-world systems development.
- [EuroRust](https://eurorust.eu/)
  - A European Rust conference covering systems programming, web development, embedded systems, and the wider ecosystem.
- [RustLab](https://rustlab.it/)
  - An international Rust conference featuring technical talks, workshops, and community activities.
- [Rust Nation UK](https://www.rustnationuk.com/)
  - A UK-based conference for Rust developers, featuring talks, workshops, and community networking.
- [Rustikon](https://rustikon.com/)
  - A Rust conference bringing together developers to share knowledge and explore the ecosystem.
- [Rust in Paris](https://rustinparis.com/)
  - A community-driven Rust conference featuring technical presentations and online participation.
- [TokioConf](https://tokioconf.com/)
  - A conference focused on asynchronous Rust, Tokio, and building high-performance production services.

### Communities

- [Rust Users Forum](https://users.rust-lang.org/)
  - The official community forum for asking questions, sharing projects, and discussing Rust programming.
- [Rust Internals Forum](https://internals.rust-lang.org/)
  - A discussion forum focused on Rust language development, compiler internals, and language design.
- [Rust Zulip](https://rust-lang.zulipchat.com/)
  - The primary chat platform for Rust project teams, contributors, and community discussions.
- [Rust Programming Language Community Discord](https://discord.gg/rust-lang-community)
  - A large community Discord server for learning Rust, getting help, and connecting with other developers.
- [r/rust](https://www.reddit.com/r/rust/)
  - A Reddit community for Rust news, discussions, questions, and project showcases.
- [Rust Community on Stack Overflow](https://stackoverflow.com/questions/tagged/rust)
  - A question-and-answer community for solving Rust programming problems.
- [Rust User Groups](https://rust-lang.org/community/)
  - A directory of local Rust meetups and community events around the world.

### Podcasts

- [Rustacean Station](https://rustacean-station.org/)
  - A community-driven podcast featuring interviews, discussions, and technical deep dives into the Rust ecosystem.
- [Rust in Production](https://corrode.dev/podcast/)
  - Explores how companies use Rust in production through interviews with engineers and technology leaders.
- [Netstack.FM](https://netstack.fm/)
  - A podcast about Rust, networking, protocols, and the engineers building modern internet infrastructure.
- [Oxide and Friends](https://oxide-and-friends.transistor.fm/)
  - Covers systems engineering, operating systems, hardware, infrastructure, and low-level technologies, including Rust.

### Newsletters

- [This Week in Rust](https://this-week-in-rust.org/)
  - A weekly newsletter covering Rust releases, community updates, new projects, articles, events, and job opportunities.
- [Rust Bytes](https://weeklyrust.substack.com/)
  - A weekly curated newsletter featuring Rust news, technical discussions, project spotlights, and learning resources.
- [Awesome Rust Weekly](https://rust.libhunt.com/newsletter)
  - A weekly collection of Rust projects, libraries, tools, releases, and ecosystem news.
- [The Embedded Rustacean](https://theembeddedrustacean.com/)
  - A newsletter focused on embedded Rust, microcontrollers, hardware projects, and embedded development tutorials.
- [Rust Trends](https://rust-trends.com/)
  - A newsletter highlighting Rust ecosystem developments, industry adoption, technical articles, and emerging projects.
- [How To Code It](https://www.howtocodeit.com/newsletter)
  - A newsletter sharing practical Rust programming techniques, software architecture insights, and engineering discussions.

**[⬆ Back to Top](#contents)**

## Contributing

Contributions are welcome!

Please read the [Contributing Guidelines](CONTRIBUTING.md) before submitting a project or suggesting an improvement.

Make sure your submission is relevant to the Rust ecosystem, properly documented, and placed in the most appropriate category.

**[⬆ Back to Top](#contents)**

## License

This project is licensed under the [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

**[⬆ Back to Top](#contents)**
