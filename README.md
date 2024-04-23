# telnetlib2

In [PEP 594](https://peps.python.org/pep-0594/#telnetlib), telnetlib has been deprecated. The library has been removed from Python 3.13 onwards.

telnetlib2 is telnetlib (the module, the test suite and the documentation) extracted from the [cpython git repo](https://github.com/python/cpython/) keeping the git history intact.

PEP 594 [suggests](https://peps.python.org/pep-0594/#deprecated-modules) the following alternatives:

- [telnetlib3](https://pypi.org/project/telnetlib3/)
- [Exscript](https://pypi.org/project/Exscript/)

Both are great projects, but neither of the two are drop-in replacements for telnetlib. telnetlib3 uses [asyncio](https://docs.python.org/3/library/asyncio.html), which would mean existing code using telnetlib would need a rewrite. Exscript has a much larger scope covering several protocols including telnet. The syntax is very different, which would also mean a rewrite of existing code using telnetlib.

