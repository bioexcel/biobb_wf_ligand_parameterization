[![](https://readthedocs.org/projects/biobb-wf-ligand-parameterization/badge/?version=latest)](https://biobb-wf-ligand-parameterization.readthedocs.io/en/latest/?badge=latest)
[![](https://mybinder.org/badge_logo.svg)](https://bioexcel-binder.tsi.ebi.ac.uk/v2/gh/bioexcel/biobb_wf_ligand_parameterization/master?filepath=biobb_wf_ligand_parameterization%2Fnotebooks%2Fbiobb_ligand_parameterization_tutorial.ipynb)

# Automatic Ligand parameterization tutorial using BioExcel Building Blocks (biobb)

***

This tutorial aims to illustrate the process of **ligand parameterization** for a **small molecule**, step by step, using the **BioExcel Building Blocks library (biobb)**. The particular example used is the **Sulfasalazine** protein (3-letter code SAS), used to treat rheumatoid arthritis, ulcerative colitis, and Crohn's disease.

**OpenBabel and ACPype** packages are used to **add hydrogens, energetically minimize the structure**, and **generate parameters** for the **GROMACS** package. With *Generalized Amber Force Field (GAFF) forcefield and AM1-BCC* charges.

***

## Settings

### Biobb modules used

* [biobb_io](https://github.com/bioexcel/biobb_io): Tools to fetch data to be consumed by the rest of the Biobb building blocks.
* [biobb_chemistry](https://github.com/bioexcel/biobb_chemistry): Tools to manipulate chemical data.

### Auxiliar libraries used

* [nb_conda_kernels](https://github.com/Anaconda-Platform/nb_conda_kernels): Enables a Jupyter Notebook or JupyterLab application in one conda environment to access kernels for Python, R, and other languages found in other environments.
* [nglview](http://nglviewer.org/#nglview): Jupyter/IPython widget to interactively view molecular structures and trajectories in notebooks.
* [ipywidgets](https://github.com/jupyter-widgets/ipywidgets): Interactive HTML widgets for Jupyter notebooks and the IPython kernel.

### Conda Installation and Launch

```console
git clone https://github.com/bioexcel/biobb_wf_ligand_parameterization.git
cd biobb_wf_ligand_parameterization
conda env create -f conda_env/environment.yml
conda activate biobb_ligand_parameterization_tutorial
jupyter-nbextension enable --py --user widgetsnbextension
jupyter-nbextension enable --py --user nglview
jupyter-notebook biobb_wf_ligand_parameterization/notebooks/biobb_ligand_parameterization_tutorial.ipynb
```

***

## Tutorial

Click here to [view tutorial in Read the Docs](https://biobb-wf-ligand-parameterization.readthedocs.io/en/latest/index.html)

***

## Version
2021.2

## Copyright & Licensing
This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).

* (c) 2015-2021 [Barcelona Supercomputing Center](https://www.bsc.es/)
* (c) 2015-2021 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)

Licensed under the
[Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.

![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
