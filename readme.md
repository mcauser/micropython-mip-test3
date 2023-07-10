# MicroPython MIP test 3

One in a series of example repos to test various mpremote mip installation patterns.

#### Install

```
$ mpremote mip install github:mcauser/micropython-mip-test3

Install github:mcauser/micropython-mip-test3
Installing github:mcauser/micropython-mip-test3/package.json to /lib
Installing: /lib/test3/__init__.py
Done
```

GitHub        | Device
:-------------|:----------------------
/src/test3.py | /lib/test3/__init__.py

```
$ mpremote repl

>>> from test3 import Test3
>>> t3 = Test3()
test3 __init__
>>> t3.main()
test3 main
```

#### Install examples

```
$ mpremote mip install github:mcauser/micropython-mip-test3/examples.json

Install github:mcauser/micropython-mip-test3/examples.json
Installing github:mcauser/micropython-mip-test3/examples.json to /lib
Installing: /lib/test3/test3_basic.py
Installing: /lib/test3/test3_complex.py
Done
```

GitHub                     | Device
:--------------------------|:---------------------------
/examples/test3_basic.py   | /lib/test3/test3_basic.py
/examples/test3_complex.py | /lib/test3/test3_complex.py

```
$ mpremote repl

>>> import test3.test3_basic
test3 __init__
test3 basic
>>> import test3.test3_complex
test3 __init__
test3 complex
```
