# 🤖 AI Data Analysis Agent

An AI-powered data analysis system that allows users to analyze CSV datasets using **natural-language questions**. The agent uses the **Gemini API** to understand the user's request, select the appropriate analysis tool, execute the analysis using Python and Pandas, and present the results through a Streamlit interface.

## 📌 Problem Statement

Business users depend on data analysts for repetitive data exploration and reporting, making the process time-consuming and inefficient.

## 🎯 Objective

To build an AI-powered data analysis agent that enables users to interact with datasets using natural language and automatically perform common data-analysis tasks.

## ✨ Features

* 📂 Upload and analyze CSV datasets
* 💬 Ask questions in natural language
* 🤖 AI-based analysis tool selection
* 📊 Calculate statistical measures
* 🔍 Detect missing values
* 📋 Find unique/categorical values
* 📈 Generate histograms
* 📊 Generate bar charts
* 🔗 Calculate correlation between numerical columns
* 📉 Generate scatter plots
* 📝 Provide easy-to-understand analysis results
* 🌐 Interactive Streamlit web interface

## 🛠️ Technologies Used

**Python, Pandas, Gemini API, Matplotlib, Streamlit, Google Colab, Pyngrok**

## 🔧 Analysis Tools

The agent can automatically select from the following tools:

1. `inspect_dataset` – Inspects dataset structure
2. `calculate_statistics` – Calculates statistics for one numerical column
3. `calculate_multiple_statistics` – Calculates statistics for multiple numerical columns
4. `find_missing_values` – Detects missing values
5. `get_unique_values` – Finds unique values
6. `dataset_overview` – Provides an overall dataset summary
7. `plot_histogram` – Generates a histogram
8. `plot_bar_chart` – Generates a bar chart
9. `calculate_correlation` – Calculates correlation between two numerical columns
10. `plot_scatter` – Generates a scatter plot

## 🔄 How It Works

```text
User
  ↓
Natural-Language Question
  ↓
Gemini AI Agent
  ↓
Select Appropriate Analysis Tool
  ↓
Python + Pandas
  ↓
Perform Analysis
  ↓
Matplotlib Visualization / Result
  ↓
Streamlit Interface
  ↓
User-Friendly Insight
```

## 🧩 Example

**User Question:**

> What is the correlation between Age and Income?

**Agent Process:**

```text
User Question
     ↓
Gemini identifies required analysis
     ↓
calculate_correlation
     ↓
Pandas calculates correlation
     ↓
Result generated
     ↓
Insight presented to user
```

## 📋 Requirements

* Python 3.10+
* Google Gemini API key
* CSV dataset
* Internet connection
* Google Colab or Jupyter Notebook
* Required Python libraries:

  * `google-genai`
  * `pandas`
  * `matplotlib`
  * `streamlit`
  * `pyngrok`

## 🚀 Installation

Install the required libraries:

```bash
pip install -U google-genai pandas matplotlib streamlit pyngrok
```

## 🔑 Gemini API Key

Create a Gemini API key and set it as an environment variable.

```python
import os
import getpass

os.environ["GEMINI_API_KEY"] = getpass.getpass(
    "Enter your Gemini API key: "
)
```

**Never upload your API key to GitHub.**

## ▶️ Running the Project

### 1. Upload a CSV dataset

The application accepts CSV files for analysis.

### 2. Start the Streamlit application

```bash
streamlit run app.py
```

### 3. Open the Streamlit interface

Upload your dataset, enter a natural-language question, and click **Analyze**.

## 💡 Sample Questions

```text
How many rows and columns are in the dataset?

What is the average Age?

Give statistics for Age and Income.

Are there any missing values?

What are the unique values in Gender?

Show the distribution of Age.

Show a bar chart of Gender.

What is the correlation between Age and Income?

Show a scatter plot of Age and Income.

Give me an overview of the dataset.
```

## 📁 Project Structure

```text
AI-Data-Analysis-Agent/
│
├── app.py
├── README.md
└── dataset.csv
```

## 🔮 Future Enhancements

* Add SQL database support
* Implement Gemini Function Calling
* Add more advanced visualizations
* Add anomaly detection
* Add automated report generation
* Support Excel files
* Add multiple AI agents for specialized analysis
* Deploy the application online

## 🎓 Project Outcome

The project demonstrates how **Generative AI can be combined with traditional Python data-analysis tools** to create an interactive AI agent capable of understanding natural-language requests and performing data-analysis tasks automatically.

## 👩‍💻 Author

**Laasya Reddy Kadumuri**

BTech Computer Science Engineering
Interested in **Artificial Intelligence, Generative AI, Agentic AI, and Software Development**.
