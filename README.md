# James Allen's Linguistic Transformation Analysis

**Author(s):** [Your Name]

This repository contains a comprehensive Natural Language Processing (NLP) analysis of James Allen's philosophical transformation as evidenced through his writings.

## 📖 Project Description

This project analyzes the linguistic differences between James Allen's two philosophical works:

- **"As a Man Thinketh" (1903)** - Focus on self-mastery and thought control
- **"The Way of Peace" (1907)** - Focus on ego dissolution and surrender

Using computational text analysis, we measure:

1. **Vocabulary shifts** - From "thought/mind/character" to "peace/love/soul"
2. **Agent pronoun reduction** - 67% decrease in individual pronouns (I, he, man)
3. **Verb valence changes** - From active (build, master) to surrender (release, dissolve)
4. **Semantic inversions** - "Self" transforms from tool to enemy
5. **Peace frequency** - 4.4x increase in peace-related language

**Key Finding:** James Allen's ego death is measurable in grammar itself—peace requires dissolution, not mastery.

---

## 📁 Repository Structure

```
ProjectTemplate/
├── README.md                           # Project documentation
├── requirements.txt                    # Python dependencies
├── data/                              # Raw text data
│   └── [Place book text files here]
├── notebooks/                         # Jupyter notebooks
│   ├── 1_Main_Analysis.ipynb         # Primary linguistic analysis
│   ├── 2_Exploratory_Analysis.ipynb  # Initial data exploration
│   └── 3_Visualizations.ipynb        # Additional visualizations
├── results/                           # Output files
│   ├── figures/                      # Generated visualizations
│   └── tables/                       # CSV exports and tables
└── slides/                            # Presentation materials
```

---

## 📑 Project Outline

### Analysis Pipeline

1. **Data Loading & Preprocessing** (Notebook 2)

   - Load text files from Project Gutenberg
   - Remove headers/footers
   - Normalize whitespace

2. **Text Tokenization** (Notebook 2)

   - Simple regex-based tokenization
   - Preserve all word forms naturally
   - No lemmatization (to track exact usage patterns)

3. **Distinctive Words Analysis** (Notebook 1)

   - Log-likelihood (G²) statistical testing
   - Identify words distinctive to each book
   - Frequency normalization (per 10,000 words)

4. **Pronoun Analysis** (Notebook 1)

   - Agent pronoun tracking (I, me, my, he, him, his, man)
   - First, second, third person comparison
   - Confound control analysis

5. **Semantic Analysis** (Notebook 1)

   - Verb valence (active vs. surrender verbs)
   - Self-context analysis (positive vs. negative)
   - Emotional intensity metrics

6. **Statistical Validation** (Notebook 1)

   - Bootstrap confidence intervals (95%)
   - Significance testing

7. **Visualization** (Notebook 3)
   - Comparative bar charts
   - Philosophical trinity analysis
   - Peace metric visualization

---

## 🚀 Environment Setup

Before starting, please **fork this repository** and create a fresh Python virtual environment.  
All required libraries are listed in `requirements.txt`.

> ⚠️ If you encounter errors during `pip install`, try removing the version pinning for the failing package(s) in `requirements.txt`.  
> On Apple M1/M2 systems you may also need to install additional system packages (the “M1 shizzle”).

---

### macOS / Linux (bash/zsh)

```bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
source .venv/bin/activate

# Upgrade pip and install dependencies
pip install --upgrade pip
pip install -r requirements.txt
```

### Windows (PowerShell)

```powershell
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
.venv\Scripts\Activate.ps1

# Upgrade pip and install dependencies
pip install --upgrade pip
pip install -r requirements.txt
```

---

## 📊 Key Results

### Quantitative Findings

| Metric              | Book 1 (Thinketh) | Book 2 (Peace)   | Change      |
| ------------------- | ----------------- | ---------------- | ----------- |
| **Agent Pronouns**  | 654.3 per 10k     | 217.8 per 10k    | **-67%**    |
| **Peace Frequency** | 9.4 per 10k       | 41.4 per 10k     | **+4.4x**   |
| **Active Verbs**    | High              | Lower            | Decreases   |
| **Surrender Verbs** | Low               | Higher           | Increases   |
| **Self Sentiment**  | Positive (tool)   | Negative (enemy) | **Inverts** |

### Visualizations

All visualizations are saved in [`results/figures/`](./results/figures/):

- `slide3_philosophical_trinity.png` - Truth, Love, Self frequency comparison
- `slide5_agent_pronouns.png` - Agent pronoun vanishing analysis
- `slide6_confound_control.png` - Rhetorical vs philosophical change
- `slide7_mechanism.png` - Verb valence & self-context shifts
- `slide8_peace_metric.png` - Peace frequency & emotional intensity

---

## 📓 Notebooks

### 1. Main Analysis (`1_Main_Analysis.ipynb`)

Primary analytical notebook containing:

- Complete text processing pipeline
- Log-likelihood distinctive words analysis
- Agent pronoun analysis with visualizations
- Confound control testing
- Verb valence and semantic inversion analysis
- Peace metric calculation
- Bootstrap statistical validation
- Summary and data export

### 2. Exploratory Data Analysis (`2_Exploratory_Analysis.ipynb`)

Initial data exploration including:

- Text statistics and basic metrics
- Word frequency distributions
- Vocabulary diversity analysis
- Preliminary visualizations

### 3. Advanced Visualizations (`3_Visualizations.ipynb`)

Additional visual analysis:

- Interactive plots
- Word clouds
- Comparative analysis charts
- Publication-ready figures

---

## 🛠️ Technologies Used

- **Python 3.11+**
- **pandas** - Data manipulation and analysis
- **numpy** - Numerical computing
- **matplotlib** - Static visualizations
- **seaborn** - Statistical data visualization
- **pathlib** - File path operations
- **collections.Counter** - Word frequency counting
- **re** - Regular expressions for text processing

---

## 📈 Interpretation Notes

### The Philosophical Trinity

Allen's transformation centers on three core concepts:

1. **TRUTH** (96.9 per 10k in Book 2) - From intellectual mastery to divine understanding
2. **LOVE** (87.0 per 10k in Book 2) - From self-control to universal compassion
3. **SELF** (84.6 per 10k in Book 2) - From tool of mastery to enemy to transcend

**Peace** (41.4 per 10k) emerges as the natural outcome when these three align.

### Statistical Robustness

All findings confirmed with 95% bootstrap confidence intervals:

- Agent pronoun reduction: Statistically significant (non-overlapping CIs)
- Peace frequency increase: Highly significant
- Changes are not due to sampling variation

---

## 🚀 Getting Started

1. **Clone this repository**

   ```bash
   git clone <your-repo-url>
   cd ProjectTemplate
   ```

2. **Set up virtual environment** (see Environment Setup above)

3. **Place data files** in the `data/` folder:

   - `As a man thinketh.txt`
   - `The way of Peace.txt`

4. **Run notebooks** in order:
   - Start with `2_Exploratory_Analysis.ipynb`
   - Then `1_Main_Analysis.ipynb`
   - Finally `3_Visualizations.ipynb`

---

## 📝 Citation

If you use this analysis in your research, please cite:

```
[Your Name]. (2025). James Allen's Linguistic Transformation Analysis:
Measuring Philosophical Change Through Computational Text Analysis.


## 🙏 Acknowledgments

- Text sources: Project Gutenberg
- Inspiration: James Allen's philosophical works
- Statistical methods: Log-likelihood ratio testing, bootstrap resampling

# Upgrade pip and install dependencies

python -m pip install --upgrade pip
pip install -r requirements.txt

```

### Windows (Git Bash)

```bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
source .venv/Scripts/activate

# Upgrade pip and install dependencies
python -m pip install --upgrade pip
pip install -r requirements.txt
```
