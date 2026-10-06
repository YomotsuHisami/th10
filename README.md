This repo is uploaded on behalf of [@SteinsGateON](https://space.bilibili.com/34714121).

# th10

[![QQ Group 1124121427](https://img.shields.io/badge/QQ%20Group-1124121427-12B7F5?logo=tencentqq)](https://qm.qq.com/q/eeUrxIltug?from=tim)

A high-fidelity, portable reimplementation of 東方風神録　～ Mountain of Faith ver 1.00a.

## Layout

- `th10_web/`: TH10 game, SDL runtime, launcher integration, documentation, and source tests.
- `portable/`: shared GLES renderer, numeric compatibility code, input code, build orchestration, and validation tools.
- `tools/`: the pinned Emscripten installer and its metadata.

## Build

Install the pinned toolchain, then build the browser runtime:

```powershell
python tools/download-emscripten.py
node portable/build.mjs --th10
```

Build outputs are written below `th10_web/artifacts/` and are intentionally not tracked.

## Assets and licensing

This repository does not include original Touhou executable, data, music, replay, or save files. A runnable package must be assembled locally from files you are legally allowed to use.

## License

This project is licensed under the MIT License.
