# Python for Economics Course

A course on Python and programming for PhD candidates in economics

If you are going to *develop* from this repository, go to the [development guide](README_DEV.md).

## Installing Python for Economics Course:

Remember to follow these instructions from within your preferred virtual environment:

    conda create -n pyeco python=3.13
    conda activate pyeco

The first way  is to clone the repository and do a local installation:

    git clone https://github.com/tiagoft/pyeco.git
    cd pyeco
    pip install .

The second way is to install directly:

    pip install git+https://github.com/tiagoft/pyeco.git

To uninstall, use:

    pip uninstall pyeco

## Usage

To find all implemented commands, run:

    pyeco-cli --help
