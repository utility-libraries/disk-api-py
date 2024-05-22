# fs-api
An API... but in the filesystem

> [!IMPORTANT]
> This is only an idea at the current point in time

## Basic Idea

```python
from fsapi import FSAPI

api = FSAPI()

@api.get("/index")
def index():
    return f"Hello World"


if __name__ == '__main__':
    api.run(mount="~/api/")
```
```shell
$ cat ~/api/index
Hello World
```
