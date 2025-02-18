# Soluci-n-Guia-2
name: Python application

on: [push]

jobs:
  build:

    runs-on: ubuntu-latest

    steps:
    - name: Checkout repository
      uses: actions/checkout@v2

    - name: Setup Python
      uses: actions/setup-python@v2
      with:
        python-version: '3.x'

    - name: Run Python script
      run: |
        python main.py
