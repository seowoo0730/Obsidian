```Python
import packages.echo
packages.echo.echo_test()
# echo
```

## `__all__`

```Python
# __init__.py
__all__ = ['echo']
```

```Python
from packages import *
from packages.echo import echo_test
echo_test()
render_test()
# echo
# NameError: name 'render_test' is not defined
```

> [!info] PyPI · The Python Package Index  
> The Python Package Index (PyPI) is a repository of software for the Python programming language.  
> [https://pypi.org/](https://pypi.org/)