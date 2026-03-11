# lighter-wasm
Lighter Wasm required for working with Lighter in JS/TS

Compiled directly from https://github.com/elliottech/lighter-go

Check how to set it up here: https://github.com/ccxt/ccxt/wiki/FAQ#how-to-use-the-lighter-exchange-in-ccxt

- CCXT is using the WASM binary built from the official package and it can be downloaded here or built from the source
- You also need to provide the path to `exec_wasm.js`, you can either download it from the same repo or check the path to your local file (assuming Go is installed)

Example

```Javascript
lighter = new ccxt.lighter({
	'options': {
		'libraryPath': '/user/cjg/Git/lighter-wasm/lighter.wasm',
		'wasmExecPath': '/opt/homebrew/opt/go/libexec/lib/wasm/wasm_exec.js'
	}
})
```

If you need help or encounter any difficulties during the process, the CCXT team is ready to assist you.
