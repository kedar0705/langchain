# Migrating to `langchain.experimental`

We are moving any experimental components of langchain, or components with vulnerability issues, into `langchain_experimental`.
This guide covers how to migrate.

## Installation

Previously:

`pip install -U langchain`

Now:

`pip install -U langchain langchain_experimental`

## PALChain

Previously:

`from langchain.chains import PALChain`

Now:

`from langchain_experimental.pal_chain import PALChain`

## SQLDatabaseChain

Previously:

`from langchain.chains import SQLDatabaseChain`

Now:

`from langchain_experimental.sql import SQLDatabaseChain`

## `load_prompt` for Python files

Note: this only applies if you want to load Python files as prompts.
If you want to load json/yaml files, no change is needed.

Previously:

`from langchain.prompts import load_prompt`

Now:

`from langchain_experimental.prompts import load_prompt`
