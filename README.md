# weighting
Derive weights so that the distributions of two populations are proportional in N-dimensional space

This is a pure C code based on the original C++ code by Carlos Cunha;
significant parts of the code are essentially unchanged.  A python wrapper is
provided

# python code

Currently the python code just calls out to the C code.  I plan to make a proper
C extension in the future

For an example, see the test code weighting.test_gaussians()

## Installing python code
```bash
python setup.py install --prefix=/some/path
python setup.py install --prefix=~/local

# The python code calls out to the C code, so make
# sure the executable is in your path
```

# C code

## compilation

Currently codes for different number of dimensions are compiled separately. The following
make different executables 

```bash
# makes calcweights5
make ndim=5

# makes calcweights1
make ndim=1

# installation
make ndim=2 install
make ndim=5 install prefix=~/local

# uninstall
make ndim=5 uninstall prefix=~/local
```
