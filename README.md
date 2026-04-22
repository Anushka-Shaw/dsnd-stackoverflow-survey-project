# Stack Overflow Developer Survey 2025 — What Makes a High-Earning Developer?

## Project Motivation
This project analyzes the Stack Overflow Annual Developer Survey 2025 to understand
what factors drive developer salaries. Following the CRISP-DM data science process,
we explore 49,000+ responses to answer 4 key business questions about developer compensation.

## Questions Explored
1. Does years of experience strongly predict salary?
2. Does education level matter for developer compensation?
3. Are remote workers paid differently than office workers?
4. Can we build a model to predict whether a developer earns above the median salary?

## Libraries Used
- `pandas` — data loading and manipulation
- `numpy` — numerical operations
- `matplotlib` — data visualization
- `seaborn` — statistical plots
- `scikit-learn` — machine learning (Random Forest, model evaluation)
- `pathlib` — file path handling

## Files in This Repository
| File | Description |
|------|-------------|
| `analysis.ipynb` | Main Jupyter notebook with full CRISP-DM analysis |
| `survey_results_public.csv` | Raw survey data (49,191 responses, 172 columns) |
| `survey_results_schema.csv` | Column descriptions for the survey dataset |
| `salary_distribution.png` | Plot: raw vs filtered salary distribution |
| `salary_by_education.png` | Plot: median salary by education level |
| `salary_by_experience.png` | Plot: median salary by years of experience |
| `salary_by_remote.png` | Plot: median salary by work arrangement |
| `model_results.png` | Plot: confusion matrix and feature importance |
| `README.md` | This file |

## Summary of Results
- **Experience is the #1 predictor** of salary — developers with 30+ years earn
  nearly 3x more ($115,720) than those just starting out ($40,586)
- **Remote workers earn significantly more** — $97,476 median vs $59,030 for in-person
- **Education has less impact than expected** — PhD holders earn the most ($92,812)
  but the gap between degree levels is smaller than experience gaps
- **Our Random Forest model achieved 62% accuracy** at predicting whether a developer
  earns above the median salary of $82,709 — well above the 50% random baseline

## How to Run
1. Clone this repository
2. Place `survey_results_public.csv` in the same folder as `analysis.ipynb`
3. Install dependencies:
pip install pandas numpy matplotlib seaborn scikit-learn
4. Open `analysis.ipynb` in Jupyter or VS Code and run all cells

## Acknowledgements
- Dataset: [Stack Overflow Annual Developer Survey 2025](https://survey.stackoverflow.co/)
- Inspiration: [Stack Overflow Survey Results](https://survey.stackoverflow.co/2024/)
- Project framework: Udacity Data Scientist Nanodegree