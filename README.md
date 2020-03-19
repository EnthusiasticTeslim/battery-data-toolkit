# Battery Data Extractor 

This directory contains utilities for converting battery testing data files from native formats
to a standardized HDF5 file.

It also contains some scripts that run these utilities on datasets available to the ASOH project.

## Installation

The package can be installed with pip,
which will install the minimal amount of packages needed for this library
to function:

```bash
pip install -r requirements.txt
pip install -e .
```

For development purposes, we recommend installing the library and 
all requirements
using Anaconda rather than pip. 
Anaconda reliably gathers compatible 
versions of all libraries and we have the versions of the libraries
fixed in that development environment.
Install the environment using: 

`conda env create --file environment.yml --force`

## Project Organization

The `scripts` folder holds code that processes different datasets used by our collaboration. 

Any logic that is general enough to warrant re-use is moved into the `batdata` Python package.

The Python package also holds the schemas, which are described in 
[`schemas.py`](./batdata/schemas.py).
