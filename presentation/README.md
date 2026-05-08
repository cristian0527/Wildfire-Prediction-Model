# Overview

Our presentation's slides are all in the "presentation.qmd" file. This file uses the data from `../data` and images from `./images` to render. To preview these files, ensure you installed all dependencies before rendering with Quarto (see following sections). The raw data comes from the source dataset described in "../data/README.md" and the processed files are generated from the "../scripts" notebooks. Also, note that we cite where we got the images we didn't create in the "presentation.qmd" file.

### Dependencies
0. [Quarto](https://quarto.org/)
0. [Python](https://www.python.org/)
    * Here we use version 3.12, as documented in the ".python-version" file.
0. Python package manager like [uv](https://docs.astral.sh/uv/) to install the dependencies in "pyproject.toml".
    * We track "uv.lock" through Git following the developer's [recommendation](https://docs.astral.sh/uv/guides/projects/#uvlock)
    * After [installing](https://docs.astral.sh/uv/concepts/projects/sync/#creating-the-lockfile) the dependencies through `uv sync`, make sure to activate the environment by running `source .venv/bin/activate` within the "presentation" directory.

### Rendering
After installing all the dependencies, you can render "presentation.qmd" like you would any other Quarto presentation document. To preview, you can run `quarto preview presentation.qmd` within the "presentation" directory.