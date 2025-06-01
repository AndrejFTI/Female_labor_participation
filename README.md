# Female Labor Force Participation Project

## Motivation

Understanding what influences **female labor force participation** is critical for informed policymaking, especially in the context of global development. Using World Bank data, this project explores the relationship between gender-specific factors like **female school enrollment** and **adolescent fertility**, alongside gender-agnostic factors like **urbanization**, **poverty**, and **GDP** as predictors for female labor force participation.

Full project write-up on Medium can be found [here](https://medium.com/@andrejsemail/what-drives-female-labor-force-participation-in-slovakia-90680ba27335):gi

---

## Libraries Used

- `pandas` – data manipulation  
- `numpy` – numerical operations  
- `matplotlib` / `seaborn` – data visualization  
- `scikit-learn` – modeling and evaluation  
  
---

## Repository Structure

| File / Folder               | Description |
|----------------------------|-------------|
| `notebook.ipynb`           | Main analysis and modeling notebook |
| `data/`                    | Contains raw dataset |
| `README.md`                | Project overview and documentation |
| `requirements.txt`         | List of Python packages needed to run the notebook |

---

## Summary of Results

- Linear regression was used to explore the effect of adolescent fertility, education, and economic factors on female labor force participation.
- The model had **low predictive performance (R² = -4.73)**, suggesting that:
  - The relationships between features and target are likely non-linear
  - Additional or alternative features may be necessary
- Feature importance from linear regression indicated:
  - **Urban population %** had the strongest (positive) coefficient
  - **Adolescent fertility** and **GDP per capita** also had noticeable impacts
- Correlation analysis showed:
  - **School enrollment (education)** had a **negative correlation (-0.33)** with labor force participation, potentially reflecting delayed workforce entry due to education, or a time lag effect not captured within the dataset’s limited time range.
  - **Adolescent fertility** had a **positive correlation (0.35)** with labor force participation, possibly indicating earlier workforce entry following early motherhood.

> These results should be interpreted with caution due to poor model fit. Further research and more robust modeling are recommended.

---

## Acknowledgements

- [World Bank Open Data](https://data.worldbank.org/) – source of all datasets