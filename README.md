# Eaglercraft 26.2

This is a browser build of Minecraft 26.2, with the Java game source and the tools used to compile it to WebAssembly. The main game code is in `game/`; the browser targets and build scripts are in `platform-teavm/`, `target_teavm_wasm_gc/` and `wasm-toolchain/`.

## Build

Use Java 25 and Node.js from the repository folder. Install the Node package first, then run one of these:

```sh
npm ci
npm run build:dev:web
```

That makes a local hosted build under `target_teavm_wasm_gc/build/web`. The script marks its output local-only.

For a standalone HTML file, run:

```sh
npm run build:single
```

By default, this writes `eaglercraft-26.2-single.html` in the repository folder. The commands are listed in `package.json`.

## Licences

Minecraft and its resources are copyright Mojang Studios. This checkout also contains third-party components; keep their own licence and notice files with them, and check the relevant terms before sharing source or builds.
