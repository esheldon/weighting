# weighting
derive weights so that the distributiins of two populations are proportional in N-dimensional space

This is a pure C code based on the original C++ code by Carlos Cunha.  A python
wrapper is provided

# python code

Currently the python code just calls out to the C code.  I plan to make a proper
C extension in the future

## Installing python code
```
python setup.py install --prefix=/some/path
python setup.py install --prefix=~/local
```

# C code

## compilation

Currently codes for different number of dimensions are compiled separately.  e.g.

```bash
make ndim=5
make ndim=1

make ndim=2 install

make ndim=5 install prefix=~/local
make ndim=5 uninstall prefix=~/local
```
