# Package Managers in Python

They range from simple installers to "all-in-one" project managers. 

As of 2026, uv is the recommended default for most modern Python projects due to its extreme speed and ability to replace multiple older tools.

## pip 

The standard installer that comes with Python. It is simple but lacks built-in "lock files" for reproducibility and doesn't manage virtual environments on its own.

## PyPI

This is not a manager; it is the repository (the store) where Python packages are hosted. All managers listed here (except Conda) pull their packages from PyPI.

## uv 

A new, lightning-fast manager written in Rust. It is a "drop-in" replacement for pip but also manages Python versions, virtual environments, and lock files.

## Poetry

A popular "all-in-one" tool that focuses on a structured workflow and reproducibility. It's great for building libraries but can be slower than uv.

## Conda

Specialized for Data Science and Machine Learning. Unlike the others, it handles non-Python dependencies like C++ libraries or CUDA.

## PDM

A modern manager that adheres strictly to the latest Python packaging standards. It is a lightweight alternative to Poetry.
