# MAGEE
Mixed-model Association tests for GEne-Environment interactions

## Description
MAGEE is an R package for gene-environment interaction (GEI) tests and joint tests (testing the marginal genetic effects and GEI effects simultaneously) for genome-wide association studies (GWAS) and large-scale sequencing studies <a href="https://doi.org/10.1002/gepi.22351">Wang et al. (2020)</a>. Based on the generalized linear mixed models (GLMMs) <a href="https://doi.org/10.1080/01621459.1993.10594284">Breslow and Clayton (1993)</a>, the tests within the MAGEE framework are highly efficient. 

For GWAS, MAGEE performs single-variant tests for GEI and joint effects. For rare variant analysis, MAGEE performs group tests based on user-defined variant sets. The group-based tests include two GEI tests and three joint tests: interaction variance component test (IV), interaction hybrid test using Fisher's method (IF), joint variance component test (JV), joint hybrid test using Fisher's method (JF), and joint hybrid test using double Fisher's procedures (JD). Before running MAGEE for analyzing the data across the whole genome, a global null model that only accounts for covariates (not including any genetic main effects) is fitted. The model should be fitted using the R package <a href="https://CRAN.R-project.org/package=GMMAT">GMMAT</a> proposed by <a href="https://doi.org/10.1016/j.ajhg.2016.02.012">Chen et al. (2016)</a>. See the <a href="https://github.com/large-scale-gxe-methods/MAGEE/blob/master/inst/doc/MAGEE.pdf">vignettes</a> for details.

## Installing
See Section 3.2 of the <a href="https://github.com/large-scale-gxe-methods/MAGEE/blob/master/inst/doc/MAGEE.pdf">vignette</a>.

For optimal computational performance, it is recommended to use an R version configured with the Intel Math Kernel Library (or other fast BLAS/LAPACK libraries). See the <a href="https://www.intel.com/content/www/us/en/developer/articles/technical/using-onemkl-with-r.html">instructions</a> on building R with Intel MKL.

## Version
The current version is 1.4.5 (February 11, 2026).

## License
This software is licensed under GPL (>= 3).

## Contact
Please refer to the R help document of MAGEE for specific questions about each function. For comments, suggestions, bug reports and questions, please contact Han Chen (hanchenphd AT gmail.com). For bug reports, please include an example to reproduce the problem without having to access your confidential data.

## Acknowledgments
This work was supported by National Institutes of Health (NIH) grants R00 HL130593 and R01 HL145025.

## References
<p>Please cite
<li>Wang X, Lim E, Liu C, Sung YJ, Rao DC, Morrison AC, Boerwinkle E, Manning AK, Chen H. (2020) Efficient gene-environment interaction tests for large biobank-scale sequencing studies. <em>Genetic Epidemiology</em> <b>44(8):</b> 908-923. PMID: <a href="https://www.ncbi.nlm.nih.gov/pubmed/32864785">32864785</a>. PMCID: <a href="https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7754763/">PMC7754763</a>. DOI: <a href="https://doi.org/10.1002/gepi.22351">10.1002/gepi.22351</a>.</li></p>
<p>If you use MAGEE meta-analysis, please also cite
<li>Wang X, Pham DT, Westerman KE, Pan C, Manning AK, Chen H. (2022) Genomic summary statistics and meta-analysis for set-based gene-environment interaction tests in large-scale sequencing studies. <em>medRxiv</em> 2022.05.08.22274819. DOI: <a href="https://doi.org/10.1101/2022.05.08.22274819">https://doi.org/10.1101/2022.05.08.22274819</a>.</li></p>
