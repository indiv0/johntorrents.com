# 👷‍♀️🦀🕸️ [`johntorrents.com`](https://johntorrents.com)

<table>
  <tr>
    <td><strong>Linux</strong></td>
    <td>
      <a href="https://travis-ci.org/github/indiv0/johntorrents.com" title="Travis Build Status">
        <img src="https://img.shields.io/travis/indiv0/johntorrents.com/main?style=flat-square" alt="travis-badge"></img>
      </a>
    </td>
  </tr>
  <tr>
    <td><strong>Windows</strong></td>
    <td>
      <a href="https://ci.appveyor.com/project/indiv0/johntorrents-com" title="Appveyor Build Status">
        <img src="https://img.shields.io/appveyor/build/indiv0/johntorrents-com/main?style=flat-square" alt="appveyor-badge"></img>
      </a>
    </td>
  </tr>
  <tr>
    <td colspan="2">
      <a href="LICENSE">
        <img src="https://img.shields.io/github/license/indiv0/johntorrents.com?style=flat-square" alt="license-badge"></img>
      </a>
    </td>
  </tr>
</table>

This site is an inside joke. Don't ask.

It's based on the template for kick starting a Cloudflare worker project
using [`wasm-pack`](https://github.com/rustwasm/wasm-pack).

This project is compiled from a Rust library into WebAssembly and the resulting
worker gets published to Cloudflare's worker infrastructure.

## 🔋 Batteries Included

* [`wasm-bindgen`](https://github.com/rustwasm/wasm-bindgen) for communicating
  between WebAssembly and JavaScript.
* [`console_error_panic_hook`](https://github.com/rustwasm/console_error_panic_hook)
  for logging panic messages to the developer console.
* [`wee_alloc`](https://github.com/rustwasm/wee_alloc), an allocator optimized
  for small code size.

## 🚴 Usage

### 🐑 Clone this Repo

```
git clone https://github.com/indiv0/johntorrents.com
cd johntorrents.com
```

### 🛠️ Build with `wasm-pack build`

```
wasm-pack build
```

### 🔬 Test in Headless Browsers with `wasm-pack test`

```
wasm-pack test --headless --firefox
```
