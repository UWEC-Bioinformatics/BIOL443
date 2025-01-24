# BIOL443

To prepare the conda environment, run the following in a terminal (not a VS Code terminal):

``` bash
mamba env create -f environment.yml
```

To use the environment to run R code blocks in an IPython Notebook:

1. Start a VS Code session (set this repo as the working directory)
2. In a terminal, activate the environment: `conda activate biol443`
3. Start R: `R`
4. Install the IRkernel spec: `IRkernel::installspec()`
5. Quit the R session: `q()` (don't save the workspace)
6. Open the test notebook `R4DS_test.ipynb`
7. Click Select Kernel > Jupyter Kernel... > R (the one with biol443 in the path)

If you ever need to install a new R package, make sure you install it with conda/mamba, and then restart the Jupyter kernel.