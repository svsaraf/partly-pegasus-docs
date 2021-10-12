# Pegasus Documentation

Documentation for [SaaS Pegasus: the Django SaaS Boilerplate](https://www.saaspegasus.com/).

The latest docs can be found at [docs.saaspegasus.com](https://docs.saaspegasus.com/).

This project uses [Sphinx](https://www.sphinx-doc.org/).

## Installation

Install using your favorite version [from Sphinx's options](https://www.sphinx-doc.org/en/master/usage/installation.html).

The maintainer uses the pip version via `pip install -r requirements.txt`

## Building Docs

To build docs run `make html`.

## Viewing docs locally

You can use python to serve your docs locally after building them:

```python
cd _build/html
python -m http.server 8080
```

The docs should now be visible at [http://localhost:8080](http://localhost:8080).

The following one-liner may be useful to clean, build, and serve the docs. Run this in the `_build/html` folder.

```
cd ../../ && rm -r _build && make html && cd _build/html/ && python -m http.server 8080
```

## Deployment

Deployment is handled by Netlify. The latest master is automatically deployed.
