# Loom: Go + WebAssembly UI Framework (Experimental)

**Loom** is an experimental UI framework for the web.

**Goal:** Build UIs with **Go** compiled to **WebAssembly (WASM)**. Svelte-inspired, meaning: compile-time optimization, no virtual DOM, fast, small.

**🚨 WARNING: This is deep alpha. Expect breakage. This is research.**

## Why?

*   Go on frontend.
*   WASM speed.
*   Svelte's minimal runtime.
*   Because we can.

## How (The Gist)

1.  Write `.loom` files (HTML + Go script + CSS).
2.  `loom build` runs our custom compiler.
3.  Compiler generates Go code, raw HTML, and tiny JS glue.
4.  Go compiles to `main.wasm`.
5.  Browser loads WASM. Go code updates DOM directly via JS bridge.

## Status

MVP build in progress. Focus on:
*   Parser for `.loom`
*   `$state` reactivity
*   Surgical DOM updates (comment anchors)
*   Go ↔ JS event/state bridge
*   Basic `loom build` CLI.

## Usage

Not ready for public use yet. Code is here.

## Contribute

Got ideas? Think this is stupid/brilliant? Open an issue. Let's talk.

## License

MIT.
