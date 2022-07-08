## Install quarto

Installation procedure: https://quarto.org/docs/getting-started/installation.html

## Create a conda environment for running quarto

```
conda create -n quarto
conda activate quarto
conda install mamba
mamba install jupyterlab pandas matplotlib scipy
```

To draw Bayesian networks you could render .dot graphs:
```
pip install graphviz
```

```
export QUARTO_PYTHON=/Users/lode/opt/anaconda3/envs/quarto/bin/python
```
check with ```echo $QUARTO_PYTHON                                              
/Users/lode/opt/anaconda3/envs/quarto/bin/python```

## Optional if you want to execute R in your docs

( instead ofnstall R: https://cloud.r-project.org/, install R with conda:)

```
mamba install r-essentials r-base
mamba install -c r r-leaflet
```

## Check if quarto is working fine

Check with: ```quarto check jupyter```
