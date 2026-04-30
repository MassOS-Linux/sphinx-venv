# sphinx-venv
Prebuilt sphinx venv packages for the MassOS build system

These packages are designed for MassOS use only. They are hardcoded to the
directory that the MassOS build system expects, which is the following:
```
/root/mbs/extras/sphinx
```

But the version of the package has to match the Python version used in the
MassOS build system. So these packages have to be regenerated on a newer
version of Python.

Note that while Sphinx itself is architecture-independent, some of the Python
dependencies included in this venv distribution are compiled to native machine
code (`.so` files). Therefore the entire distribution has to be labelled as
architecture-specific. And currently x86_64 and aarch64 are the only supported
architectures (the nightly run alternates between x86_64 on odd days of the
month and aarch64 on even days of the month).
