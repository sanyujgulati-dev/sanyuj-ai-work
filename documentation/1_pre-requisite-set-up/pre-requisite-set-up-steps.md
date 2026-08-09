# Set Up
This file contains the steps for setting up and isntalling necessary extensiions.

## GIT extension
Donwload the GIT extension for extensions

## Jupyter Notebook extension
Jupyter Notebook is an open-source, web-based application that lets you create and share documents containing live code, equations, visualizations, and explanatory text. You open Jupyter Notebook in a browser, where you can write and execute code in "cells." Each notebook contains a mix of code cells and text cells, forming a complete computational narrative. Code runs through a "kernel" (e.g., IPython for Python), and outputs are displayed inline. Download and install Jupyter Notebook extension.

## UV Python Package installation
Uv is a next-generation, Rust-powered Python manager that unifies package installation, environment management, and Python version control into one ultra-fast tool. use this web site https://docs.astral.sh/uv/ to download uv and set up your virtual python environment.
After installation, run the following commands:
1. uv --verions
2. uv self update
3. uv sync

Sync command downloads all artefacts needed for creating a virtual python environment. Run this command to sync uv for each project you create.

## Set up OpenAI API key
You need to create an account in OpenAI platform for creating a API secret Key. After the key successfully created add the key to a file under your project named ".env". The Open AI API key will be added in following format:
OPENAI_API_KEY=<API Key value from OpenAI Portal>