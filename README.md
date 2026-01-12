# DZ2024_Semielasticities
The paper: [https://wiiw.ac.at/the-cyclical-behaviour-of-government-spending-for-social-protection-is-the-oecd-methodology-robust-p-6719.html](https://wiiw.ac.at/the-cyclical-behaviour-of-government-spending-for-social-protection-is-the-oecd-methodology-robust-p-6719.html)

## Codebase structure:

1. "_processing_" gets the data and creates two csv files from it for models and plotting
2. "_Visualizations_General_" is how the plots were created; _"legacy/Visualizations AUTplusDEU"_ is for the German language publication and *may* have newer settings for the plots
3. "_models_clean_" contains arima/ols/ivreg variations and their iterative implementation for the outputs that we have in the [publication](https://wiiw.ac.at/the-cyclical-behaviour-of-government-spending-for-social-protection-is-the-oecd-methodology-robust-p-6719.html)

* models_clean.Rmd can be either run (xlsx output) or knit (adjust what you need in the code; currently it will only display the real potential output tables)
* Cursor was used to shorten the code and make it more stable. The legacy code can be found in the legacy folder, but it has a very WIP flavor. Most of the models etc. are stored as files and can be uncommented (e.g. Ljung test); only the output for the major points of relevance for the paper is rendered now.

## To get the repo:

```
cd existing_repo
git remote add origin https://gitlab.wiiw.io/avarsenev/dz2024_semielasticities.git
git pull origin dev
```