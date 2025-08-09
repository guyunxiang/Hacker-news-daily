# Show HN: A Python CEL implementation (written in Rust)

**Posted by hardbyte on 2025-08-08**

I've been working on a Python library for the Common Expression Language (CEL). It serves as a wrapper around the `cel-rust` crate, which is under active development. The Python wrapper uses PyO3 and Maturin to handle the Rust-Python interop.

CEL is a safe, fast, non-Turing complete expression language ideal for configuration, validation rules, or policy engines. It allows you to evaluate user-defined logic without the security risks associated with `eval()`.

### Installation

You can install it via pip or uv:

```bash
uv tool install common-expression-language
```

### Usage

Start the REPL:

```bash
cel -i
```

Evaluate an expression directly:

```bash
cel 'size(data.things) > 1' --context '{"data": {"things": [1, 2, 3]}}'
```

### Documentation & Source

- [Documentation](https://python-common-expression-language.readthedocs.io/en/latest/)
- [Source Code](https://github.com/hardbyte/python-common-expression-language)