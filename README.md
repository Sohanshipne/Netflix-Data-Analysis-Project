 🎬 Netflix Movies Data Analysis

A Python-based exploratory data analysis (EDA) project on Netflix movie data using **Pandas**, **Matplotlib**, and **Seaborn**.



📌 Project Overview

This project analyzes a Netflix movies dataset (`mymoviedb.csv`) to uncover trends and insights about genres, popularity, ratings, and release patterns. It covers the full EDA pipeline — from data cleaning to visualization.



* Key Questions Answered

- What is the most frequent genre of movies released on Netflix?
- Which vote average category has the highest count?
- Which movie has the **highest** popularity? What is its genre?
- Which movie has the **lowest** popularity? What is its genre?
- Which year had the most movies filmed/released?


 📂 Dataset

File: `mymoviedb.csv`

| Column | Description |
|---|---|
| `Title` | Movie title |
| `Release_Date` | Release date (converted to year) |
| `Genre` | Genre(s) of the movie |
| `Vote_Average` | Average user vote score |
| `Popularity` | Popularity score |
| `Overview` | Movie description *(dropped)* |
| `Original_Language` | Language *(dropped)* |
| `Poster_Url` | Poster image URL *(dropped)* |

> Note: `Overview`, `Original_Language`, and `Poster_Url` columns were dropped as they were not needed for the analysis.



 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.x | Core programming language |
| Pandas | Data manipulation & cleaning |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical data visualization |
| Jupyter Notebook | Interactive analysis environment |



 📊 Analysis Steps

1. **Data Loading** — Load CSV using Pandas
2. **Exploration** — `.head()`, `.info()`, `.describe()`, `.duplicated()`
3. **Data Cleaning**
   - Convert `Release_Date` to year format
   - Drop irrelevant columns
   - Handle missing values with `.dropna()`
4. **Feature Engineering**
   - Categorize `Vote_Average` into: `not_popular`, `below_avg`, `average`, `popular`
   - Explode multi-genre entries into individual rows
5. **Data Visualization**
   - Genre distribution (bar chart)
   - Vote average distribution
   - Release year histogram
   - Highest & lowest popularity movies


 📈 Sample Visualizations

- **Genre Distribution** — Most common genres on Netflix
- **Vote Average Distribution** — How movies are rated overall
- **Release Year Histogram** — Year-wise movie count trend


 🚀 How to Run

1. Clone the repository
   ```bash
   git clone https://github.com/your-username/netflix-data-analysis.git
   cd netflix-data-analysis
   ```

2. Install dependencies
   ```bash
   pip install -r requirements.txt
   ```

3. Add the dataset
   - Place `mymoviedb.csv` in the root directory of the project.

4. Launch Jupyter Notebook
   ```bash
   jupyter notebook Netflix_data_analysis.ipynb
   ```



 📁 Project Structure

```
netflix-data-analysis/
│
├── Netflix_data_analysis.ipynb   # Main analysis notebook
├── mymoviedb.csv                 # Dataset (add manually)
├── requirements.txt              # Python dependencies
└── README.md                     # Project documentation
```



 📝 Notes

- The dataset file `mymoviedb.csv` is **not included** in this repository. Please source it from [Kaggle - TMDB Movies Dataset](https://www.kaggle.com/datasets/disham993/9000-movies-dataset) or your own copy.
- Run all cells in order for correct results.

---

 🙋‍♂️ Author

- GitHub: [@my-username](https://github.com/Sohanshipne)
- LinkedIn: [my-linkedin](https://linkedin.com/in/mr-sohan=shipne)

---

 📄 License

This project is open source and available under the [MIT License](LICENSE).
