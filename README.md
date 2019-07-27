# crfsuite-rs

[![Build Status](https://travis-ci.org/bosondata/crfsuite-rs.svg?branch=master)](https://travis-ci.org/bosondata/crfsuite-rs)
[![codecov](https://codecov.io/gh/bosondata/crfsuite-rs/branch/master/graph/badge.svg)](https://codecov.io/gh/bosondata/crfsuite-rs)
[![Crates.io](https://img.shields.io/crates/v/crfsuite.svg)](https://crates.io/crates/crfsuite)
[![docs.rs](https://docs.rs/crfsuite/badge.svg)](https://docs.rs/crfsuite/)
[![PyPI](https://img.shields.io/pypi/v/crfsuite)](https://pypi.org/project/crfsuite)

Rust binding to [crfsuite](https://github.com/chokkan/crfsuite)

## Installation

Add it to your ``Cargo.toml``:

```toml
[dependencies]
crfsuite = "0.2"
```

Add ``extern crate crfsuite`` to your crate root and your're good to go!

## Python package

There is also a Python package named `crfsuite`, you can install it via `pip`:

```bash
pip install -U crfsuite
```

Usage example:

```python
from crfsuite import Model

if __name__ == '__main__':
    model = Model('path/to/crfsuite/model.crf')
    tagged = model.tag(["abc", "def"])
    print(tagged)
```

## License

This work is released under the MIT license. A copy of the license is provided in the [LICENSE](./LICENSE) file.

