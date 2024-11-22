# Polartoolkit_workshop

Files for running a workshop to teach PolarToolkit

* [Documentation](https://polartoolkit.readthedocs.io/en/latest/index.html)
* [GitHub Repository](https://github.com/mdtanker/polartoolkit)
* [Poster](https://raw.githubusercontent.com/mdtanker/polartoolkit-posters/2211242154dffac74b95c2a41a20f5c68af556d2/poster_v3/polartoolkit_poster_v3.svg)

## Install

### Use PolarToolkit online (Binder)
If you don't want to install anything, you can use PolarToolkit online through our [Binder environment](https://mybinder.org/v2/gh/mdtanker/polartoolkit-binder/main?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Fmdtanker%252Fpolartoolkit%26urlpath%3Dtree%252Fpolartoolkit%252Fdocs%252Ftutorial%26branch%3Dmain), but note that nothing you create on this webpage will be saved unless you download it!

### Install locally
Ideal, you should install the software and run in locally on your computer. Make sure you have Python 3.9 or greater installed. You can check this in Terminal with `which python`. If you don't, I recommend using Miniforge to set it up, see the install instructions [here](https://github.com/conda-forge/miniforge).

There are a few ways to install PolarToolkit
#### Conda
```{note}
`conda` and `mamba` are interchangeable
```

Create a new virtual environment:
```
mamba create --name ptk --yes --force polartoolkit jupyterlab geoviews cartopy ipyleaflet --channel conda-forge
```
Activate the environment:
```
mamba activate ptk
```

#### Pip
Create a new virtual environment:

```
mamba create --name ptk --yes --force pygmt geopandas cartopy python=3.12 --channel conda-forge
```
activate the environment and use `pip` to install `polartoolkit`:

```
mamba activate ptk
pip install polartoolkit[all]
```