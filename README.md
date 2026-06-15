## Global Outcomes of Traumatic Brain Injury Across Human Development Index Strata: A Multi-Center, International, Prospective Cohort Study

[![DOI](https://zenodo.org/badge/1269677570.svg)](https://doi.org/10.5281/zenodo.20694959)

**Authors:** Joseph G. Nugent, M.D., M.P.H., M.H.S., C.P.H.<sup>1</sup>; Hao Tan, M.D.<sup>3</sup>; Brittany Stedelin, M.D.<sup>1</sup>; Caleb Nerison, M.D.<sup>2</sup>; Zoe Teton, M.D.<sup>4</sup>; Saud K. Zaidan, B.S.<sup>1</sup>; Andreas K. Demetriades, MB.BChir., M.Phil.<sup>5</sup>; Adam A. Dmytriw, M.D., M.P.H.<sup>6</sup>; Megan Still, M.D.<sup>7</sup>; Hazem S. Ghaith, M.D.<sup>1</sup>; Claire Zeigler, M.D., M.P.H.<sup>1</sup>; Barbara Lazio, M.D.<sup>1</sup>; Ahmed Negida, M.D., Ph.D<sup>8</sup>; Ahmed M. Raslan, M.D.<sup>1</sup> and GNS-1 Collaborators (Ahmad Ghassan Hammouri (Palestine); Ahmad Ozair (India); Alaa Mohammad Hamdan (Syria); Ali Haider Bangash (Pakistan); Ankur Bajaj (India); Ansam Ghzawi (Jordan); Chee Yang Tan (Malaysia); Enoch Ogbonnaya Uche (Nigeria); Haytham Osman (Sudan); Michael D. Cusimano (Canada), Abdelhakim Khellaf (Canada), Ignatius Esene (Cameroon); Ivan D. Lozada-Martinez (Colombia); Jhon Bocanegra (Peru); Konstantinos Gousias (Germany); Luis Rafael Moscote-Salazar (Colombia); Mohamed Gedi Sheikhow (Somalia); Muhammed Elhadi (Libya); Mustapha Amnir (Mauritania); Enow Awah Georges Stevens (Cameroon); Nesrine Ben Hadj Dahman (Tunisia); Arsene Daniel Nyalundja (Democratic Republic of Congo); Obanife Henry Olayere (Nigeria); Oumaïma Outani (Morocco); Pierfrancesco Lapolla (Italy); Ruben Martin-Laez (Spain); Sadi A. Abukhalaf (Palestine); Sudipta Kumer Mukherjee (Bangladesh); Wenjin Chen (China), Rimantas Vilcinis (Lithuania))

1. Department of Neurosurgery, Oregon Health & Science University, Portland, OR, USA
2. Lexington Medical Center, West Columbia, SC, USA
3. Department of Neurosurgery, Emory University School of Medicine, Atlanta, GA, USA
4. Department of Neurosurgery, UCLA Health, Los Angeles, CA, USA
5. Department of Clinical Neurosciences, Edinburgh University Hospitals, Edinburgh, UK
6. Massachusetts General Hospital, Harvard University, Boston, MA, USA
7. Department of Neurosurgery, University of Florida, Gainesville, FL, USA
8. Department of Neurology, Virginia Commonwealth University, Richmond, VA, USA

## Data Availability

The dataset in this repository is a de-identified, pre-processed version of the study’s analytic sample from patient records collected as part of the GNS-I study, approved by the Oregon Health & Science University (OHSU) Institutional Review Board (IRB #00021490). All direct and quasi-identifiers have been removed or generalized in accordance with the HIPAA Safe Harbor method (45 CFR §164.514(b)). No information sufficient to re-identify any individual is knowingly present in this repository. A data dictionary describing each variable, its type, and coding scheme is provided in `GNS-I_Data Dictionary.docx`. All variables are labeled in `R`, and categorical variables are coded as factors with the levels explicitly labeled, as shown in the Quarto document output. Formal requests for the full dataset or for identifying metrics should be sent to the study’s data guarantor (<a href= “mailto:nugentj@ohsu.edu”>nugentj@ohsu.edu</a>) and principal investigator (<a href= “mailto:raslana@ohsu.edu”>raslana@ohsu.edu</a>), accompanied by proof of ethical approval from the applicant’s home institution. Following approval of each individual request, the data will be shared directly with the interested party via a secure file-sharing system, including all raw data collected, the processing code used to generate the final analytic sample from the raw data, the final analytic dataset, as well as a codebook for both datasets within 30 days of the written request. Additionally, the original study protocol and details regarding the collaborative are available online at <a href= “https://www.globalneurosurg.org/”>globalneurosurg.org</a>.

## Code Availability

This repository contains the `R` code used to generate the descriptive and analytic results, as well as all tables and figures from the associated study. The knitted Quarto files contain session information detailing the required `R` version, packages used in the analysis, and their associated URLs, provided they are packages not available on CRAN. Packages or dependencies that are not available on CRAN or GitHub can be found in the CRAN Archive, referenced by the appropriate version number. Additionally, the generated output relies on a proprietary package created by the study’s primary author that is not publicly maintained on GitHub; as such, an archived version is included in this repository.

## Instructions for Use

Once the repository is downloaded and the associated packages listed in the session information section of the document footers are installed (along with the archived version of `jgntools`), the Quarto Markdown files may be knit, as they reference the analytic data file located in the same directory. Note that for `jgntools` to load properly, some archived packages may need to be installed, as detailed above.

## Repository File Contents

- **GNS-I Nature Medicine Analysis.qmd**: Quarto Markdown document used to generate the outputs for the entirety of the study, the only exception being the `xgboost` exploratory results.
- **GNS-I Nature Medicine Analysis.html**: Knitted version of the above.
- **GNS-I xgboost.qmd**: Quarto Markdown document used to generate the results of the `xgboost` exploratory analysis for all the study’s relevant outcomes.
- **GNS-I xgboost.html**: Knitted version of the above.
- **GNS-I_Analytic Dataset.RData**: The de-identified and pre-processed GNS-I analytic dataset.
- **GNS-I_Collaborators.docx**: A complete list of all the study’s collaborators and centers contributing data to the study.
- **GNS-I_Data Dictionary.docx**: The associated data dictionary listing all variable names and descriptions. Factor variables are coded with levels containing clear definitions.
- **jgntools.zip**: An archived version of the primary author’s personal package used for pre-processing and generation of many output tables and figures.
- **references.bib**: Associated references included in the analysis Qmd file.

## Data Use and Citation

Any work that uses or builds upon these data or code must include an appropriate citation, as well as notification of the study’s data guarantor (<a href= “mailto:nugentj@ohsu.edu”>nugentj@ohsu.edu</a>) and principal investigator (<a href= “mailto:raslana@ohsu.edu”>raslana@ohsu.edu</a>). Any attempt to re-identify individuals in this dataset is strictly prohibited.
