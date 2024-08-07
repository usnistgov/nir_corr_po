# Correlations of Near-Infrared Spectra to Bulk Properties in Polyolefins, using Principal Component Analysis

This repository supports the following peer-reviewed manuscript:

> Bradley P. Sutliff, Shailja Goyal, Tyler B. Martin, Peter A. Beaucage,
> Debra J. Audus, and Sara V. Orski,
> "Correlating Near-Infrared Spectra to Bulk Properties in Polyolefins"
> *Macromolecules* 2024, 57. 5. 2329-2338
> DOI: https://doi.org/10.1021/acs.macromol.3c02290

which uses functional principal component analysis to connect
near-visible infrared (NIR) spectra of polyolefins with physical
properties to enable better sorting of these materials.

The repository is intended for the following use cases:

- Illustrate key ideas from the submitted manuscript including using functional
  principal component analysis and sliced inverse regression for correlating
  NIR with physical properties.
- Reproduce figures from our submitted manuscript
- Allow for full reproducibility of the data in the submitted manuscript

## Running the notebook

The included notebook `nir-corr-po.ipynb` allows the user to reproduce all of
the figures in the corresponding submitted manuscript, using the corresponding
data. The notebook is setup to walk the user through each of the preprocessing
and analyzing steps, generating corresponding figures along the way. All code
is written in Python and requires Python == 3.9. It can be used on any
operating system. Other requirements are listed in `requirements.txt`.

The code can either be run locally or in [Google Colab].

### Run notebook locally (option 1)

#### Clone the code

First clone the code via

```bash
git clone https://github.com/usnistgov/nir_corr_po.git
```

and navigate to the directory where the repository lives

```bash
cd nir_corr_po
```

Next, one needs to create a virtual environment. This can be done using Python
virtual environments or with Anaconda. Both options are listed below.

#### Create a Python virtual environment (option 1)

First, make sure you are using Python 3.9.

```bash
python3 -m venv env
```

where `env` is the location of the virtual environment

Activate the virtual environment

```bash
source env/bin/activate
```

Install dependencies

```bash
python3 -m pip install -r requirements.txt
```

#### Create a virtual environment with Anaconda (option 2)

First, install [conda]. Then run the following in a conda-enabled terminal.

```bash
conda env create -f environment.yml
```

This yml file will automatically name the new environment `ncp`.

If you are using conda>=4.6, activate the virtual environment via

```bash
conda activate ncp
```

Otherwise, see the [conda docs].

#### Run the notebook

The Jupyter notebook can be run by using the command

```bash
jupyter notebook
```

### Running notebook in Google Colab (option 2)

If you are interested in running the notebook in [Google Colab], first click on
the relevant link below. Note that these links were generated by navigating to
the notebook of interest on the nir_corr_po GitHub page, for example,
`https://github.com/usnistgov/nir_corr_po/nir-corr-po.ipynb` and then replace
`github.com` with `githubtocolab.com`.

- [nir-corr-po][nir-corr-po-colab]

This should open the notebook in Google Colab.

## Contact

Bradley P. Sutliff, PhD  
Materials Science and Engineering Division  
Material Measurement Laboratory  
National Institute of Standards and Technology  

Email: Bradley.Sutliff@nist.gov  
GitHubID: @bpsut  
Staff website: <https://www.nist.gov/people/bradley-sutliff>  

## How to cite

If you use the code, please cite our submitted manuscript:

> Bradley P. Sutliff, Shailja Goyal, Tyler B. Martin, Peter A. Beaucage,
> Debra J. Audus, and Sara V. Orski,
> "Correlating Near-Infrared Spectra to Bulk Properties in Polyolefins"
> *Macromolecules* 2024, 57. 5. 2329-2338
> DOI: https://doi.org/10.1021/acs.macromol.3c02290

If you use the data, please cite:

> Sutliff, Bradley; Goyal, Shailja; Martin, Tyler; Beaucage, Peter;
> Audus, Debra; Orski, Sara. Correlations of Near-Infrared Spectra to
> Bulk Properties in Polyolefins, using Principal Component Analysis,
> National Institute of Standards and Technology (2023),
> <https://doi.org/10.18434/mds2-3022> (Accessed YYYY-MM-DD)

## Future updates and maintenance

There is no intent to update/maintain this repository once it is released to
the public, given that it is intended to reproduce published figures and
analysis that should not change over time.

<!-- links -->
[Google Colab]: https://colab.research.google.com/
[conda]: https://www.anaconda.com
[conda docs]: https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html
[nir-corr-po-colab]: https://githubtocolab.com/usnistgov/nir_corr_po/blob/main/nir-corr-po.ipynb
