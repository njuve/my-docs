---
title: "How to use Logging"
date: 2020-02-21T20:30:23+09:00
draft: true
---

# Summary

Official document is [logging — Logging facility for Python](https://docs.python.org/3/library/logging.html).
Nice article written in japanese is [Pythonでロギングを学ぼう](https://qiita.com/__init__/items/91e5841ed53d55a7895e).

Main functions in `logging` are:

| Level      | When                               |
| ---------- | ---------------------------------- |
| `debug`    | Detailed information                |
| `info`     | Report expected working            |
| `warning`  | Report unexpected working          |
| `error`    | More serius                        |
| `critical` | The program can't continue working |

Using `basicConfig` we can save logs into a file.


# Example

```python
import logging
logging.basicConfig(
    filename=FILENAME, level=logging.DEBUG
)
logging.debug(FILENAME)
logging.info("hoge")
```
