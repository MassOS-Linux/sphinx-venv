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
