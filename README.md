# Presidential Election Donations Analysis

## Project Overview
This project analyzes over 30 million donation records from the 2020 U.S. Presidential Election to understand candidate funding, donor contributions, and the impact of small donations. The analysis includes computing total funds received per candidate, identifying unique contributors, and measuring the influence of small donors.

## Dataset
The dataset contains records of campaign contributions, including donor names, donation amounts, and candidate names. Key attributes include:
- **Candidate Name** (`cand_nm`)
- **Contributor Name** (`contbr_nm`)
- **Contribution Amount** (`contb_receipt_amt`)

## Key Findings
- **Total Donations Analyzed:** 100,000+ records
- **Top Funded Candidates:**
  - Joseph R. Biden: **$3.71M**
  - Donald J. Trump: **$2.77M**
  - Bernie Sanders: **$452K**
- **Unique Contributors:**
  - Joe Biden: **32,308**
  - Donald Trump: **34,783**
  - Bernie Sanders: **12,449**
- **Small Contributions Impact:** Donations of **$200 or less** accounted for **$2.75M (33.3%)** of total contributions.

## Technologies Used
- **Big Data Processing:** Apache Spark (PySpark)
- **Cloud Computing:** AWS EC2
- **Data Analysis:** Python (Pandas, NumPy)

## Implementation Steps
1. Loaded the dataset and cleaned the data.
2. Used PySpark to process large-scale donations efficiently.
3. Aggregated data to calculate total donations, mean/median values, and small-donor impact.
4. Visualized key insights for better interpretation.

## Running the Project
### Locally
1. Install dependencies:
   ```bash
   pip install pyspark pandas
   ```
2. Run the analysis script:
   ```bash
   python analysis.py
   ```

### On AWS EC2
1. Launch an EC2 instance and install Apache Spark.
2. Upload the dataset to the instance.
3. Run PySpark in Spark Shell:
   ```bash
   spark-submit analysis.py
   ```

## Future Improvements
- Expand analysis to include time-series trends in donations.
- Integrate additional visualization tools such as Tableau or Power BI.
- Automate real-time data updates using AWS Lambda.

## Author
Kush Patel  
https://github.com/KushPatel313

## License
This project is licensed under the MIT License.

