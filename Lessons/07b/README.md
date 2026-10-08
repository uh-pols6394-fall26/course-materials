# POLS 6394 — 07b: Functions and Lists

Materials for Thursday, October 8.

## Start here

1. Open `07b-slides.html` for the rendered slides. The source is `07b-slides.qmd`.
2. Open `07b-workbook.qmd` and keep it open during class.
3. Work only in this project during the lesson. It doesn't depend on an earlier Posit Cloud project.

## Files and folders

- `07b-slides.qmd` and `07b-slides.html`: slide source and rendered slides
- `07b-slides.css`: slide layout for code beside a plot
- `07b-workbook.qmd`: the student workbook and record of the class meeting
- `Data/state_policy/cspp_states.csv`: state policy liberalism and public opinion, one row per state-year
- `Data/state_policy/regions/`: the same data split into one file per region, with no region column, for the lists section

The policy liberalism measure (`pollib_median`) is from Caughey and Warshaw,
[The Dynamics of State Policy Liberalism, 1936–2014](https://doi.org/10.1111/ajps.12219)
(2016), distributed through the Correlates of State Policy Project. See the
[CSPP codebook](https://ippsr.msu.edu/sites/default/files/cspp/codebook_2-6.pdf#page=165).

Rendered workbook output and RStudio session files are ignored because they can be regenerated.

Before the lab, save `policy_trend()` and `region_mean()` in `R/07b-functions.R` and load them with `source()`.
