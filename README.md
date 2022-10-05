# nodeconfeu22
Augmenting Node.JS with WebAssembly-- NodeConf EU 2022 Lyrath Estate, Kilkenny, IE

# Building the Rust code into Wasm

```bash
cd wasm-module
cargo build --target=wasm32-wasi --release
cp target/wasm32-wasi/release/wasm-module.wasm ..
```

# Running the JS/Wasm

**Note:** Requires Node 18.x.x

```
 node --experimental-wasi-unstable-preview1 run-wasm.js
```

# Talk Slides

[on Google Slides](https://docs.google.com/presentation/d/1hibXu9VdkwqkPCIG6X0Y4Csu4siPUoPeyCSrPFB_5ZQ/edit?usp=sharing)