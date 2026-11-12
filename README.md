# kedgeway-demo

A deliberately outdated Soroban contract. It exists so [kedgeway](https://github.com/Klorenn/kedgeway) has something to diagnose and fix in public.

What is wrong on purpose:

- `soroban-sdk = "21.7.6"` (current major is 28)
- `stellar-cli` pinned to 21.5.0 in the workflow
- `wasm32-unknown-unknown` target instead of `wasm32v1-none`
- Rust 1.79.0 pinned, below the 1.84.0 Stellar requires

Try it:

```bash
npx kedgeway diagnose Klorenn/kedgeway-demo
```

Pull requests labelled `kedgeway` are opened by `kedgeway pr`.
