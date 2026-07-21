
# Netflix Movie Data Analysis

An exploratory data analysis (EDA) project on a Netflix movie dataset of nearly 9,800 titles, built with Python. The goal is to clean the data and answer practical business questions about genres, ratings, popularity, and release trends.

Maintained by **Chetan Parmar**.

---

## Project overview

Netflix is well known for its work in data science, AI, and machine learning, especially the recommendation models that read customer behaviour and viewing patterns. In this project we take the role of a data analyst with a dataset of more than 9,000 movies and answer key questions that help drive informed business decisions.

The full workflow covers loading the data, inspecting it, cleaning and reshaping it, and finally visualising the answers.

---

## Dataset

| Detail | Value |
|--------|-------|
| File | `mymoviedb.csv` |
| Rows | 9,827 movies |
| Columns | 9 |
| Quality | No missing values, no duplicates |

**Original columns:** Release_Date, Title, Overview, Popularity, Vote_Count, Vote_Average, Original_Language, Genre, Poster_Url

---

## Questions answered

1. What is the most frequent genre of movies released on Netflix?
2. Which category holds the highest number of votes in the Vote_Average column?
3. What movie got the highest popularity, and what is its genre?
4. What movie got the lowest popularity, and what is its genre?
5. Which year had the most movies filmed?

---

## Key findings

- **Most frequent genre:** Drama leads the library, appearing in about 14.5 percent of all genre entries, ahead of Comedy and Action (out of 19 genres).
- **Vote average:** After grouping ratings into four bands (not_popular, below_avg, average, popular), Drama also dominates the popular category.
- **Highest popularity:** `Spider-Man: No Way Home` (2021), an Action, Adventure, and Science Fiction title, with a popularity score of about 5,084.
- **Lowest popularity:** `The United States vs. Billie Holiday` and `Threads`, both at a popularity score of about 13.35.
- **Most productive year:** 2021 had the most releases in the dataset, followed by 2018 and 2017.

---

## Data cleaning steps

1. Converted `Release_Date` to datetime and extracted only the year.
2. Dropped columns not needed for analysis: `Overview`, `Original_Language`, `Poster_Url`.
3. Binned `Vote_Average` into four categories using quartile edges.
4. Split the comma separated `Genre` values and exploded the data so each row holds a single genre.
5. Cast `Genre` to a category type and removed any remaining nulls.

---

## Tools and libraries

- **Language:** Python 3
- **Libraries:** pandas, NumPy, Matplotlib, Seaborn
- **Environment:** Jupyter Notebook / Google Colab

---

## Repository contents

```
Netflix Movie Data Analysis/
|-- Netflix_Movie_Data_Analysis.ipynb   # Full analysis notebook
|-- mymoviedb.csv                       # Source dataset
|-- Netflix Movie Data Analysis.pdf     # Project brief and presentation
|-- README.md                           # You are here
```

---

## How to run

1. Clone the repository and open the folder.
2. Install the libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. Launch the notebook:
   ```bash
   jupyter notebook Netflix_Movie_Data_Analysis.ipynb
   ```
   Or open it directly in Google Colab.
4. Run the cells top to bottom. The notebook downloads the dataset automatically if `mymoviedb.csv` is not present.

---

## Author

**Chetan Parmar**

GitHub: [@ChetanParmarHQ](https://github.com/ChetanParmarHQ)

---

*This project is part of a wider Python portfolio focused on data analysis and real-world problem solving.*
