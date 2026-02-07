# Netflix Exploratory Data Analysis 📊

An in-depth exploratory data analysis of Netflix's content catalog, investigating trends in movie durations, genre distributions, and content characteristics over time.

[![Python](https://img.shields.io/badge/python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 🎯 Project Overview

This project analyzes Netflix's content catalog to uncover insights about:
- **Movie duration trends** over the past decades
- **Genre distributions** and their impact on content length
- **Content characteristics** across different categories
- **Platform evolution** and content strategy

### Key Question
**Are movies getting shorter over time?**

Through data analysis and visualization, we explore this hypothesis and discover the factors influencing average movie durations on Netflix.

---

## 📈 Key Findings

### 1. Movie Duration Trends (2011-2020)
- Average movie duration shows a **declining trend** from 103 minutes (2011) to 90 minutes (2020)
- The trend becomes more pronounced in recent years
- However, the decline isn't uniform across all genres

### 2. Genre Impact
The analysis reveals that shorter content is primarily driven by specific genres:

| Genre | Typical Duration | Impact |
|-------|-----------------|--------|
| **Children** | 20-45 minutes | High concentration of short content |
| **Documentaries** | 30-90 minutes | Variable, often shorter than features |
| **Stand-Up** | 45-75 minutes | Typically under 90 minutes |
| **Feature Films** | 90-150 minutes | Traditional movie lengths |

### 3. Content Diversity
- Netflix hosts a **wide variety** of content types beyond traditional feature films
- Short-form content (< 60 minutes) represents a significant portion of the catalog
- Platform strategy includes children's programming, documentaries, and stand-up specials

### 4. Conclusion
**Movies aren't necessarily getting shorter** - the apparent trend is largely explained by:
- Increased diversity in content types
- Growing catalog of non-feature content
- Platform expansion into children's programming and documentaries

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Jupyter](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)

**Libraries Used:**
- `pandas` - Data manipulation and analysis
- `numpy` - Numerical computing
- `matplotlib` - Static visualizations
- `seaborn` - Statistical data visualization
- `plotly` - Interactive charts and graphs

---

## 📦 Installation

### Prerequisites
- Python 3.11 or higher
- pip package manager

### Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/utsavpaudel/Netflix-EDA.git
   cd Netflix-EDA
   ```

2. **Create a virtual environment** (recommended)
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

5. **Open the analysis notebook**
   Navigate to `notebooks/netflix_analysis.ipynb` in the Jupyter interface

---

## 📁 Project Structure

```
Netflix-EDA/
├── data/                          # Dataset directory
│   ├── netflix_data.csv          # Main Netflix catalog data
│   ├── color_data.csv            # Color mapping data
│   └── README.md                 # Data documentation
├── notebooks/                     # Jupyter notebooks
│   └── netflix_analysis.ipynb    # Main analysis notebook
├── outputs/                       # Generated outputs
│   └── figures/                  # Saved visualizations
├── workspace/                     # Original workspace (legacy)
├── requirements.txt               # Python dependencies
├── .gitignore                    # Git ignore rules
├── LICENSE                       # MIT License
└── README.md                     # This file
```

---

## 🚀 Usage

### Running the Analysis

1. **Start Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

2. **Open the notebook**
   Navigate to `notebooks/netflix_analysis.ipynb`

3. **Run all cells**
   - Use `Cell > Run All` to execute the complete analysis
   - Or run cells individually to explore step by step

### Exploring the Data

```python
import pandas as pd

# Load the Netflix data
netflix_df = pd.read_csv('data/netflix_data.csv')

# View basic statistics
print(netflix_df.describe())

# Check data types
print(netflix_df.info())

# Explore unique values
print(netflix_df['type'].value_counts())
print(netflix_df['genre'].value_counts())
```

### Creating Visualizations

The notebook includes various visualizations:
- **Line plots** for temporal trends
- **Scatter plots** for duration analysis
- **Color-coded visualizations** to distinguish genres
- **Distribution plots** for statistical insights

---

## 📊 Analysis Workflow

### 1. Data Loading
- Import Netflix catalog data
- Inspect data structure and quality
- Check for missing values

### 2. Data Cleaning
- Filter for movies vs. TV shows
- Select relevant columns
- Handle missing or inconsistent data

### 3. Exploratory Analysis
- Calculate summary statistics
- Identify trends in movie durations
- Analyze genre distributions

### 4. Visualization
- Create temporal trend visualizations
- Build scatter plots with genre coloring
- Generate comparative charts

### 5. Insights & Conclusions
- Interpret findings
- Answer the research question
- Identify areas for future analysis

---

## 📝 Key Insights from Visualizations

### Duration Trends
The scatter plot of movie durations over time reveals:
- **Black dots**: Feature films (90-150 minutes)
- **Red dots**: Children's content (typically < 60 minutes)
- **Blue dots**: Documentaries (wide range)
- **Green dots**: Stand-up specials (45-75 minutes)

### Genre Distribution
Short movies (< 60 minutes) are predominantly:
- Children's programming
- Documentary shorts
- Stand-up comedy specials
- Special features

This explains why the overall average duration appears to decline - it's a **composition effect** rather than traditional movies becoming shorter.

---

## 🔮 Future Enhancements

- [ ] Add analysis of TV show trends and season counts
- [ ] Explore content additions by country and region
- [ ] Analyze director and cast data for patterns
- [ ] Create interactive dashboards with Plotly/Dash
- [ ] Include sentiment analysis of content descriptions
- [ ] Compare Netflix data with other streaming platforms
- [ ] Time series forecasting for content trends
- [ ] Network analysis of cast and director collaborations

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingAnalysis`)
3. Commit your changes (`git commit -m 'Add new analysis'`)
4. Push to the branch (`git push origin feature/AmazingAnalysis`)
5. Open a Pull Request

### Ideas for Contributions
- Additional visualizations
- Statistical tests and modeling
- New data sources integration
- Interactive dashboard development
- Documentation improvements

---

## 📚 Learning Resources

This project demonstrates key data analysis skills:
- **Data manipulation** with pandas
- **Data visualization** with matplotlib
- **Exploratory analysis** techniques
- **Statistical thinking** and hypothesis testing
- **Jupyter notebook** best practices

Perfect for:
- Data science portfolio projects
- Learning Python data analysis
- Practicing visualization techniques
- Understanding real-world datasets

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

**Utsav Paudel**
- GitHub: [@utsavpaudel](https://github.com/utsavpaudel)
- Email: utsavpaudel111@gmail.com
- LinkedIn: [utsavpaudel](https://www.linkedin.com/in/utsavpaudel/)

---

## 🙏 Acknowledgments

- Netflix data sourced from publicly available datasets
- Inspired by DataCamp's data analysis projects
- Built with the Python data science ecosystem

---

## 📧 Contact

For questions, suggestions, or collaboration opportunities, feel free to reach out!

---

⭐ **If you find this analysis interesting, please consider starring the repository!**
