# SSC Data Science and Analytics Workshop 2022
 
[Intro to Databases in Industry: Data Cleaning, Querying, and Modeling at Scale](https://ssc.ca/en/meetings/annual/2022-annual-meeting/workshops/data-science-and-analytics)

Speakers:
- **Rodolfo Lourenzutti**, University of British Columbia
- **Arman Seyed-Ahmadi**, University of British Columbia
- **Diego Ardila**, Shopify

## Workshop notebooks

 - [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/armanawn/ssc-workshop-databases-2022/blob/main/intro-to-sql.ipynb#offline=1) [Intro to SQL](intro-to-sql.ipynb)
 - [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/armanawn/ssc-workshop-databases-2022/blob/main/r-to-sql.ipynb#offline=1) [R to SQL](r-to-sql.ipynb)
 - [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/armanawn/ssc-workshop-databases-2022/blob/main/intro-to-dimension-modeling.ipynb#offline=1) [Intro to dimensional modeling](intro-to-dimension-modeling.ipynb)

## Setup instructions

### Recreating databases locally

You can install PostgreSQL on your own machine and load the database dump files provided in the `databases/` folder to locally recreate the databases used in the workshop for further practicing. The instructions to do so are provided [here](local-setup-instructions.ipynb).

### Notebook environment

The Jupyter notebooks in this repository use a few packages to run SQL commands within the Python environment of the notebooks, which are all provided in the [`environment.yml`](environment.yml). In order to reproduce this environment and make it accessible to Jupyter Lab, you need to install the `nb_conda_kernels` package in your `base` environment (or whichever environment Jupyter Lab is installed in) using the following command in your terminal:

```
conda install nb_conda_kernels
```

Then run the following command to recreate the environment

```
conda env create -f environment.yml
```

A new environment called `ssc2022` should appear in the list of kernels when you launch Jupyter Lab on your computer.

## License

© 2022 Arman Seyed-Ahmadi, Rodolfo Lourenzutti, Diego Ardila

Software licensed under [the MIT License](https://spdx.org/licenses/MIT.html), non-software content licensed under [the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0) License](https://creativecommons.org/licenses/by-nc-sa/4.0/). See the [license file](LICENSE.md) for more information.