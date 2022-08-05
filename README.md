# rbm_basic
basic implementation of rules-based-model for pathogen identification from mNGS data


The script `rbm_basic.R` runs the basic RBM approach for identification of pathogens from mNGS data. It applies negative-binomial background correction to CZ ID data, identifies outlier organisms, and then filters based on a list of known pathogens.

Required inputs include the CZ ID `Sample Overview .csv` file and a directory containing `Sample Taxon Reports .csv` files (one file per sample). Examples of these files can be found in the `data` directory.

The `idseqr` code for processing the CZ ID reports and applying negative-binomial background correction comes from work developed by Jack Kamm, original github repo here: https://github.com/czbiohub/idseqr