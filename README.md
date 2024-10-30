# SEC-FInancial-Statements-Analysis

## Introduction

The Financial Statement Data Set is a comprehensive resource created by the U.S. Securities and Exchange Commission (SEC) to facilitate the analysis and consumption of financial data submitted by public companies. This dataset is derived from the EX-101 attachments to various filings, which utilize the eXtensible Business Reporting Language (XBRL) to present structured financial information.

## Key Features of the Dataset
The dataset includes quarterly and annual numeric data from primary financial statements, which encompass:

1. Balance Sheet
2. IncomeStatement
3. CashFlowStatement
4. Changesin Equity
5. Comprehensive Income

## Structure
The dataset consists of four key components:

1. **Submission Data Set (SUB)**: Contains records for each XBRL submission, providing essential information about the filing entity and the submission itself.

2. **Number Data Set (NUM)**: Includes individual numeric values reported in the primary financial statements, detailing every line item from each submission.

3. **Tag Data Set (TAG)**: Provides metadata about the tags used in the submissions, including documentation labels, taxonomy versions, and tag attributes.

4. **Presentation Data Set (PRE)**: Offers insights into how tags and corresponding numbers were presented in the financial statements, including their sequence and structure.

**Update Frequency**: The Financial Statement Data Set is updated quarterly, incorporating data from filings submitted after the close of business on the last day of the quarter. This ensures users have access to the most recent financial information available.

## Analysis


### 1. Analyze financial statements for companies. Financial Statement Comparison allows analysts and investors to compare financial statements of different companies, aiding in benchmarking and performance evaluation.

#### Interpretaion of Results

**Company Comparisons**:

The financial statement comparison for the year 2021 includes three main metrics: Assets, Liabilities, and Revenue for various companies. These metrics provide a snapshot of the financial health of companies, offering insight into their financial positions relative to one another.

1. Wells Fargo & Company:
Liabilities: Wells Fargo stands out significantly, with liabilities amounting to 3.535 trillion USD. This is by far the highest liability figure among all companies in the dataset. This could indicate substantial financial commitments or debt, which may or may not be offset by equally strong asset and revenue generation. Investors would likely want to assess whether this large liability burden is sustainable given the company's operations and industry.

2. Bank of Nova Scotia:
Although not listed here for revenue or assets, if included in previous outputs, Bank of Nova Scotia has significant financial figures in liabilities and revenue, which would also be critical for comparison and evaluation.
Asset-Rich Companies:

3. Toll Brothers Inc. has 11.5 billion USD in assets, which is one of the larger asset figures among the companies listed. This suggests strong asset management, possibly due to real estate or property holdings, a common feature for Toll Brothers given their business focus.

4. Victoria's Secret & Co. has 4.22 billion USD in assets, indicating a strong financial position in terms of the company's physical or intellectual property and other resources.

**Liabilities in Other Companies**:

Companies such as Applied Industrial Technologies Inc. and Arcosa, Inc. show liabilities of 1.37 billion USD and 754.7 million USD, respectively. While these are significant liabilities, they are on a smaller scale compared to the extreme case of Wells Fargo. These liabilities must be compared with their revenue generation capacity to assess financial sustainability.

**Benchmarking**:

Benchmarking performance involves comparing companies like Victoria's Secret & Co., Toll Brothers Inc., and others based on their asset and liability management. These companies' financial data allows investors to assess how well they manage their assets relative to their debts.

Investors may use this comparison to assess liquidity, solvency, and overall financial health. For example, companies with relatively high assets but lower liabilities (such as Victoria's Secret & Co.) might be perceived as financially healthy, while those with large liabilities relative to assets could indicate higher financial risk (e.g., Wells Fargo & Company).

**Visual Representation**:

The bar chart visualizes companies' financial metrics, with assets, liabilities, and revenue displayed for each company. This representation makes it easy to spot outliers like Wells Fargo and Bank of Nova Scotia, which have much larger liabilities or revenues compared to other companies.

Wells Fargo's towering liabilities are a major outlier, suggesting it carries significant financial burdens. Analysts would need to scrutinize this closely to understand the reasons behind such large liabilities and whether they are supported by equally strong revenues or assets.


### 2. Cluster companies based on financial health. Financial health is a function of revenue and debt, i.e. a health company will have high revenue and low debt.

#### Interpretation of Results

**Clustering Overview**:

The clustering algorithm has classified the two companies, Bank of Nova Scotia and Nomad Foods Ltd, into two distinct clusters (Cluster 0 and Cluster 1).
Both companies have zero or negligible debt, leading to an extremely low debt-to-revenue ratio for both.

**Company-Level Insights**:

1. Bank of Nova Scotia:
Total revenue is around 8.07 billion USD.
Debt-to-Revenue Ratio: 1.23e-16, which is effectively zero. This indicates that the company operates with very little or no debt relative to its revenue, placing it in Cluster 1.

  Interpretation: Based on the financial metrics, Bank of Nova Scotia appears to be in a strong financial position due to its significant revenue and minimal debt.

2. Nomad Foods Ltd:
Total revenue is around 1.3 billion USD.
Debt-to-Revenue Ratio: 7.67e-16, which is also effectively zero, placing it in Cluster 0.

  Interpretation: Nomad Foods Ltd is also in a healthy financial position with low debt, though it falls into a different cluster compared to Bank of Nova Scotia due to its lower overall revenue.


**Visual Representation**:

The scatter plot shows the total revenue on the x-axis and the debt-to-revenue ratio on the y-axis, color-coded by the clusters.

The clustering result visually separates the two companies, with Bank of Nova Scotia (Cluster 1) having a much higher revenue compared to Nomad Foods Ltd (Cluster 0), despite both having a near-zero debt-to-revenue ratio.

The color scale indicates the separation of clusters, where Cluster 0 (yellow) contains Nomad Foods Ltd and Cluster 1 (purple) contains Bank of Nova Scotia.


### 3. Identify unusual reporting patterns or significant deviations from historical data, which may indicate potential fraud or misrepresentation.

#### Interpretation of Results


**Major Companies with Significant Liabilities**:

Wells Fargo & Company/MN: This company stands out with a liability value exceeding $3.5 trillion. Such a large liability deviation could indicate major financial commitments or potential misrepresentation of debt levels.

Bank of Nova Scotia: Displays unusual patterns in both liabilities and revenue, suggesting possible inconsistencies in its financial reporting. The liability figure is very large, which can signal issues with debt management or leverage.

**Companies with Multiple Anomalies**:

AZAR International Corp. and Brady Corp. both show anomalies in both assets and liabilities. This is often a red flag since significant deviations in both metrics may point to a mismatch in their reported financial position, possibly indicating balance sheet manipulation.

Everything Blockchain, Inc., Rise Gold Corp., Sunwin Stevia International, Inc., and Toll Brothers, Inc. also show discrepancies in both assets and liabilities, suggesting irregularities in their reported figures that need further investigation.

**Companies with Asset Anomalies**:

Companies such as Macy’s Inc., Lowes Companies Inc., FNB Corp/PA/, Gatos Silver, Inc., and many others exhibit asset anomalies. This could point to overstatement or understatement of assets, leading to questions about the accuracy of their reported financial health.
Profire Energy Inc., TOMI Environmental Solutions, Inc., and Applied Industrial Technologies Inc. also show anomalies in their asset reporting. These irregularities could indicate over-valuation of assets, misreporting, or potential fraud aimed at improving the company’s balance sheet appearance.

**Potential Risks Identified**:

Liability Misreporting: Significant liability anomalies, as seen in companies like Wells Fargo and Bank of Nova Scotia, might indicate high debt or issues with managing financial obligations. These deviations raise concerns about long-term solvency and debt management.

Revenue Anomalies: Unusual revenue figures (e.g., for Nomad Foods Ltd.) can indicate inflated earnings, fraudulent reporting, or attempts to meet analyst expectations through aggressive accounting tactics. Revenue manipulation is a common tactic in cases of financial misrepresentation.

Asset Overstatement: Asset anomalies seen in companies like Macy’s Inc., Lowes Companies Inc., and others raise concerns about the accuracy of their financial positions. Companies may inflate their asset values to appear more financially stable or improve borrowing conditions.

**Interpretation of the Chart**:

The chart visualizes the companies with unusual reporting patterns across their financial metrics (assets, liabilities, revenue).

Wells Fargo and Bank of Nova Scotia are outliers, especially in terms of liabilities, which suggests major deviations from what would typically be expected.

AZAR International Corp. and other companies with both asset and liability anomalies further highlight potential red flags in their balance sheet reporting.


### 4. Analyze how corporate executives and board members are connected across different companies and perform centrality analysis. Note that this dataset directly does not contain the names of office holders for a company. This data will need to be extracted from other sources such as Form 8-K or Form 10-K, or any third-party data source.

#### Interpretation of Results

**Centrality Analysis Results**:

Executives with Highest Centrality (serving on 3 boards):

Brian S. Davis, Luc de Dobbeleer, and Jonathan Coblentz serve on 3 boards each. These executives hold key positions in multiple companies, suggesting that they have significant influence and possibly serve as critical nodes in corporate governance networks. Their involvement in more companies gives them a higher centrality score.

Executives with Moderate Centrality (serving on 2 boards):

Hunter Horsley, Mark A. Miller, Thomas E. Line, Cynthia H. Zipperle, Jae A. Evans, Ryan K. Stafford, and others serve on 2 boards. These executives are moderately connected, playing roles in multiple organizations, but their centrality is lower compared to those who serve on 3 boards.

Board Overlap and Centrality:

The fact that some executives serve on multiple boards creates a network where certain individuals may act as conduits of information or decision-making across organizations. In terms of centrality analysis, the more boards an executive is connected to, the higher their centrality within the corporate governance network.

Names of office holders for companies: The dataset provided does not directly include office holder names, but this information can be extracted from external sources such as Form 8-K or Form 10-K filings, or through third-party data aggregators (e.g., data from EDGAR or other financial data platforms). These forms usually disclose changes in leadership, board appointments, and other key executive-related data. (*check references*)

### 5. Financial Query and Report Generation via GraphRAG. The user should be able to query specific financial metrics, trends, or insights from the dataset using plain English.



