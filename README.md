<<<<<<< HEAD
# Finacial Consumer Complaints

Consumer complaints on financial products & services for Bank of America from 2017 to 2023, including the dates the complaint was submitted to the CFPB and then sent to the company, the product and issue mentioned in the complaint, and the company's response
=======
# Consumer Complaints Analysis

An exploratory data analysis of 62,000+ consumer complaints submitted to financial companies between 2017-2023. This project digs into what people complain about most, how companies respond, and which issues take forever to resolve.

## What's This About?

When consumers have problems with banks, credit cards, mortgages, or other financial products, they can file complaints with regulatory agencies. This dataset contains those complaints, and I analyzed it to find patterns in:
- What financial products get the most complaints
- How companies respond (or don't respond) to issues
- Which complaints take the longest to resolve
- Trends over time

Think of it as a health check on the financial services industry from the consumer's perspective.

## Dataset Overview

**Source:** Consumer Financial Protection Bureau (CFPB)
**Size:** 62,516 complaints
**Time Period:** May 2017 - August 2023
**Industries Covered:** Banking, Credit Cards, Mortgages, Credit Reporting, Loans, Money Transfers

**Key Features:**
- Complaint ID and submission details
- Product and issue categories
- State where complaint originated
- Company response type (closed with explanation, monetary relief, etc.)
- Response timeliness (on time vs delayed)
- Economic factors (dates for trend analysis)

## Key Findings

### 1. Credit Reporting Dominates Complaints
Credit reporting and repair services receive the most complaints by far. Issues with incorrect information on credit reports are a major pain point for consumers.

### 2. Most Companies Respond, But Not Always on Time
- Majority of complaints get closed with an explanation
- Some complaints receive monetary relief
- A subset of complaints face delayed responses (analyzed separately)

### 3. Complaint Volume Increased Over Time
Monthly complaint trends show growth over the 2017-2023 period, with some seasonal spikes.

### 4. Delayed Responses Have Patterns
Untimely responses aren't random - certain product categories and issue types consistently see delays. These patterns could indicate systemic problems in how companies handle specific complaint types.

## Project Structure

```
EDA 1/
├── Consumer_Complaints_Analysis.ipynb    # Main analysis notebook
├── Consumer Complaints Analysis.pdf      # Report with visualizations
├── Pycode.py                            # Python script version
├── Working Files/
│   ├── Consumer_Complaints.xlsx         # Dataset (4MB)
│   └── ConsumerComplaints_DataDictionary.csv
├── LICENSE
└── README.md
```

## Installation & Usage

### Prerequisites
- Python 3.8+
- Jupyter Notebook

### Setup

```bash
# Clone the repository
git clone https://github.com/Swanand33/Consumer-Complaints-EDA.git
cd Consumer-Complaints-EDA

# Install required libraries
pip install pandas matplotlib seaborn openpyxl

# Launch Jupyter Notebook
jupyter notebook Consumer_Complaints_Analysis.ipynb
```

### Running the Analysis

The notebook walks through:
1. **Data Loading & Cleaning** - Handling missing values and formatting
2. **Exploratory Analysis** - Understanding data distribution and quality
3. **Complaint Trends** - Time series analysis of complaint volume
4. **Product Analysis** - Which products get complained about most
5. **Company Response Analysis** - How companies handle complaints
6. **Untimely Response Deep Dive** - Investigating delayed responses

Just run the cells in order - the analysis builds progressively.

## Technologies Used

**Data Analysis:**
- pandas - Data manipulation
- NumPy - Numerical operations

**Visualization:**
- matplotlib - Base plotting
- seaborn - Statistical visualizations

**Data Storage:**
- Excel (openpyxl) - Dataset format

## Analysis Highlights

### Complaint Volume Over Time
Line plot showing monthly complaint trends with clear growth patterns and seasonal variations.

### Top Products by Complaint Count
Bar chart revealing which financial products cause the most consumer headaches (spoiler: credit reporting wins).

### Company Response Distribution
Breakdown of how companies typically resolve complaints - most common outcomes and their frequencies.

### Untimely Response Analysis
Multi-chart analysis investigating which complaint types and categories face the longest resolution times.

## Insights for Stakeholders

**For Consumers:**
- Know which products have the most complaints before choosing services
- Understand typical resolution times and response types
- See which issues companies handle poorly

**For Financial Companies:**
- Identify problem areas in customer service
- Benchmark response times against industry patterns
- Spot systemic issues in complaint handling

**For Regulators:**
- Track complaint trends over time
- Identify companies or products needing intervention
- Monitor response quality and timeliness

## Data Notes

- Some complaints have missing sub-issue details (filled with 'Unknown')
- Response timeliness has some missing values (filled using mode)
- Analysis focuses on aggregate patterns, not individual company performance
- Dataset spans 6+ years, so trends reflect both market changes and regulatory shifts

## Limitations

- Data only includes complaints filed through official channels
- Many consumer issues never get reported formally
- Company names are anonymized in some analyses
- Economic factors (unemployment, interest rates) not included in this dataset
- No outcome quality metrics (just whether complaint was closed)

## Future Work

If I expand this analysis:
- Add sentiment analysis on complaint narratives (if text data available)
- Build predictive model for response timeliness
- Include geographic analysis by state
- Compare pre/post pandemic complaint patterns
- Analyze complaint resolution effectiveness (beyond just "closed")

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Why I Built This

Financial services can be frustrating, and understanding complaint patterns helps everyone - consumers know what to watch for, companies know what to fix, and regulators know where to focus. Plus, working with real-world messy data is great practice for data analysis skills.

This project demonstrates:
- Cleaning and preprocessing real datasets
- Exploratory data analysis techniques
- Time series analysis
- Categorical data visualization
- Drawing actionable insights from data

---

**Data source:** CFPB Consumer Complaint Database
**Analysis period:** 2017-2023
**Last updated:** 2024
>>>>>>> 5ee0cb1 (Updated notebook and README; added requirements.txt)
