# Structive Example Collection

This repository hosts a growing set of **Structive** sample projects. Every folder is an independent, runnable example that illustrates a particular pattern—tables, charts, router usage, and more.

Because each sample references **structive.js** directly from an open CDN, no build step is required. All you need is a modern browser and a tiny static‑file server such as *Live Server*.

---
## What is Structive?
Structive is a **structure‑driven UI framework for Web Components**. Instead of imperative DOM manipulation or virtual DOM diffing, it uses:

* **Structure paths** (`items.*.name`, `regions.$1.population`, …) as first‑class citizens.
* **Implicit indices** (`$1`, `$2`, …) inside loops, so you rarely declare temporary variables.
* **Getter‑based reactivity**—plain ES classes, no proxies in user code.

The result is HTML that reads almost 1‑to‑1 with the underlying data structure, keeping boilerplate close to zero.

> **TL;DR** – If you can read the template, you already know the state shape.

---
## Quick Start (Live Server)

### 1 · Clone the repo
```bash
$ git clone https://github.com/mogera551/Structive-Example.git
$ cd Structive-Example
```

### 2 · Install *Live Server*
Choose **one** of the following methods:

| Option | Install command | Notes |
|--------|----------------|-------|
| **npm package** | `npm install -g live-server` | Works from any terminal. |
| **VS Code extension** | Search for “Live Server” → *Install* | Right‑click an HTML file → **Open with Live Server**. |

### 3 · Launch the samples

#### Terminal way (npm package)
```bash
$ live-server
# LiveServer starts at http://127.0.0.1:8080 (default)
```

#### VS Code way (extension)
*Open any `index.html`, then click **Go Live** (or right‑click → **Open with Live Server**).*  
A local server starts and your default browser opens the page.

---
## Repository Layout
```
js-benchmark/        → js-benchmark demo
radar-chart/         → SVG radar chart with editable stats
states-population/   → U.S. states population aggregator
…                    → more coming soon
```
Feel free to dive into any folder—the entry point is always an `index.html` or `*.st.html` file that you can run stand‑alone.

---
## Contributing
Pull requests with new samples or improvements are welcome!  
Just follow the existing folder structure and keep external assets CDN‑hosted whenever possible.

---
© 2025 mogera551 · MIT License

