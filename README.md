# 30 Days, 30 Languages

A build streak: **one small project every day for 30 days, each in a different programming language.**

No subject theme, the single constraint is the language. The projects lean into **graphics / rendering** and **machine learning**, because those are the ones worth showing and the ones that actually teach you something structural rather than just syntax.

Built by [F4LCON](https://github.com/itsF4LCON).

---

## The rules

- **One language per day.** Thirty days, thirty languages, no repeats beyond what the list already allows.
- **Each project is day-sized** Roughly 2 to 4 hours. If something wants to be bigger, it ships as a lighter version today and goes on a "someday" note.
- **Done means done.** A day counts as shipped only when it has:
  - its own folder,
  - its own README (what it is, how to run, a screenshot),
  - and a committed result.
- **Miss rule.** One missed day is a catch-up. Two missed days in a row breaks the streak. Weekends are buffer.
- **Lighter version pre-decided.** Every hard day has a downgrade ready (one sphere instead of a full scene, XOR instead of MNIST, hello-world-in-asm before the plasma effect) so a tired day means scaling down, not quitting.

---

## The projects

| Day | Language | Project |
|----:|----------|---------|
| 01 | C++ | Ray tracer: spheres, reflections, soft shadows, PPM out |
| 02 | Rust | Real-time Mandelbrot / Julia explorer with zoom |
| 03 | C | Software rasterizer: wireframe → shaded spinning cube |
| 04 | JavaScript | WebGL shader toy: raymarched scene |
| 05 | Zig | PPM/BMP writer rendering a fractal flame |
| 06 | Go | Perlin-noise terrain heightmap → image |
| 07 | Lua (LÖVE) | Interactive particle system (gravity / wind) |
| 08 | Python | Boids flocking simulation (pygame) |
| 09 | Nim | OpenGL triangle → textured quad |
| 10 | Julia | N-body gravity sim, animated |
| 11 | Processing / Java | Generative flow-field art |
| 12 | Python | Neural net from scratch in NumPy (XOR → MNIST) |
| 13 | Python | Draw-a-digit live classifier |
| 14 | Rust | k-means with animated convergence |
| 15 | C | Linear / logistic regression, gradient descent from zero |
| 16 | JavaScript | Browser neural net separating points live |
| 17 | Go | Decision tree / random forest on a CSV |
| 18 | C++ | Genetic algorithm evolving cars / creatures |
| 19 | Python | Q-learning agent (maze or CartPole) |
| 20 | Julia | Autodiff engine (build `grad` yourself) |
| 21 | C | Software 3D engine: load `.obj`, z-buffer, flat shading |
| 22 | Rust | Path tracer with global illumination |
| 23 | C++ | Game of Life / cellular-automata lab |
| 24 | Zig | CHIP-8 emulator (runs real ROMs) |
| 25 | WebGPU (TypeScript) | Compute-shader particle sim |
| 26 | Haskell | Functional-style ray tracer |
| 27 | Elixir | Distributed Mandelbrot across processes |
| 28 | Swift | Metal shader, animated fractal |
| 29 | Kotlin | Image filter pipeline (blur, sobel, edge-detect) |
| 30 | x86-64 Assembly (NASM) | Demoscene plasma effect |

---

## Repo layout

Everything lives in this one repo. Each day is **fully self-contained** in its own folder, its own build files, its own README, its own output, so any single day can be built on its own without touching the rest.

```
30-days-30-languages/
├── README.md                    ← this file (concept + overview)
├── .gitignore                   ← build artifacts for all 30 toolchains
├── day-01-cpp-raytracer/
│   ├── README.md                ← what it is, how to run, screenshot
│   ├── src/
│   └── output.png
├── day-02-rust-mandelbrot/
│   ├── README.md
│   ├── Cargo.toml
│   └── src/
└── ... through day-30
```

Folders are named `day-NN-lang-project` and zero-padded so they sort in order.

Day-to-day progress isn't tracked here — the commit history and the folders tell that story.
