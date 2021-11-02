# WASM (with Rust) + Vite + Svelte Monorepo
## Quick Start
### Unix

Assuming a fresh install (no node, no rust)

1. Clone the repo.
2. `cd` into repo
3. Install [nvm](https://github.com/nvm-sh/nvm#installing-and-updating), close and reopen terminal after install.
4. Run
```bash
nvm install --lts
```
5. Run to verify install
```bash
node -v
// should output something similar to
v16.13.0
```
6. This monorepo uses [yarn workspaces](https://yarnpkg.com/features/workspaces) under the hood. Install `yarn` by running
```bash
npm i -g yarn
```
7. Install [rustup + rust](https://www.rust-lang.org/tools/install)
```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
// follow installation prompts, close and reopen terminal after install.
```
8. Install [wasm-pack](https://rustwasm.github.io/wasm-pack/installer/)
```bash
curl https://rustwasm.github.io/wasm-pack/installer/init.sh -sSf | sh
```
9. If in Ubuntu or similar, you need to install a CC linker (you might already have it if you've run sudo apt-get update before), run
```bash
sudo apt-get update
sudo apt install build-essential

```
10. Yarn needs rust to be build at least once so it can cross reference dependencies in the monorepo. Run in the repo root directory
```bash
yarn rust:build
// don't panic, this might take a few seconds
```
11. Install node dependencies, run
```bash
yarn
```
12. To start the development server, run
```
yarn dev
```
13. Enjoy! Got some feedback? Open an issue, or better yet, a PR. If you enjoy this, please star this repo.

## Build


## What's next
If this gets enough attention, and there demand for it, I will create a template for sveltekit, and potentially for vue and react.