# Large-Scale Wikipedia Analytics

## 📌 Overview

**Large-Scale Wikipedia Analytics** is a distributed data processing project designed to analyze the massive volume of information available in the **English Wikipedia dataset**.

The project uses **Big Data technologies such as Hadoop, HDFS, MapReduce, and Apache Spark** to process Wikipedia articles at scale. It focuses on understanding how Wikipedia content is distributed, how it grows over time, and how different knowledge categories contribute to the overall information ecosystem.

The project demonstrates how large, unstructured datasets can be processed efficiently using distributed computing rather than traditional single-machine processing.

---

## 🎯 Objectives

- Process large-scale Wikipedia article data efficiently.
- Perform distributed text and metadata analysis.
- Analyze article growth and knowledge distribution.
- Identify the most represented knowledge categories.
- Study temporal patterns in Wikipedia content.
- Demonstrate the use of Hadoop and Spark for Big Data analytics.
- Generate meaningful statistics and visualizations from large-scale data.

---

## 📊 Dataset

The project uses the **English Wikipedia dump** provided by Wikimedia.

Typical dataset:

```text
enwiki-latest-pages-articles.xml.bz2
```

The dataset contains millions of Wikipedia articles in XML format and is several gigabytes in compressed form.

The raw data includes information such as:

- Article titles
- Article text
- Page IDs
- Revision information
- Categories and metadata

Due to the large size of the dataset, it is processed using distributed computing frameworks.

---

## 🏗️ System Architecture

```text
Wikipedia XML Dump
        │
        ▼
     HDFS
        │
        ▼
 Hadoop / MapReduce
        │
        ├── Article Statistics
        ├── Word / Text Analysis
        ├── Category Analysis
        └── Data Aggregation
        │
        ▼
   Apache Spark
        │
        ├── Data Cleaning
        ├── Transformation
        ├── SQL Analysis
        └── Large-Scale Analytics
        │
        ▼
 Results & Visualizations
```

---

## ⚙️ Technologies Used

| Technology | Purpose |
|---|---|
| **Python** | Data processing and analysis |
| **Hadoop** | Distributed storage and processing |
| **HDFS** | Storage of large Wikipedia files |
| **MapReduce** | Distributed batch processing |
| **Apache Spark** | Large-scale data processing and analytics |
| **Spark SQL** | Structured querying and aggregation |
| **Pandas** | Small-scale result analysis |
| **Matplotlib / Seaborn** | Visualization |

---

## 🔄 Processing Pipeline

### 1. Data Acquisition

The Wikipedia XML dump is downloaded from Wikimedia and stored locally before being transferred to HDFS.

### 2. Data Storage

The large dataset is uploaded to **HDFS**, allowing the data to be distributed across the Hadoop cluster.

### 3. Data Extraction

Wikipedia's XML structure is parsed to extract useful fields such as:

- Page title
- Page ID
- Article text
- Categories
- Revision information

### 4. Data Cleaning

The extracted data is cleaned by removing unnecessary markup, special characters, and irrelevant metadata.

### 5. Distributed Processing

**MapReduce** is used for large-scale computations such as:

- Article counting
- Word frequency analysis
- Category statistics
- Aggregation of article-level information

### 6. Spark Analytics

Apache Spark is used for faster and more flexible analysis of the processed dataset.

Spark operations include:

- DataFrame transformations
- Filtering
- Grouping
- Aggregation
- Spark SQL queries

### 7. Visualization

The final results are converted into meaningful charts and statistics to understand Wikipedia's knowledge distribution and growth patterns.

---

## 📈 Key Analyses

### Article Growth Analysis

Analyze how the number of Wikipedia articles changes across different time periods.

### Category Analysis

Identify which knowledge categories contain the largest number of articles.

### Text Analysis

Analyze article content to determine:

- Most frequent words
- Average article length
- Distribution of article sizes
- Common terminology

### Knowledge Distribution

Compare the representation of different subject areas and identify highly represented or underrepresented categories.

### Temporal Analysis

Study changes in Wikipedia content over time to identify periods of rapid knowledge growth.

---

## 💡 Key Features

- Handles **large-scale Wikipedia data**
- Uses **distributed storage with HDFS**
- Uses **MapReduce for parallel processing**
- Uses **Apache Spark for high-speed analytics**
- Supports structured and unstructured data analysis
- Produces interpretable statistical results and visualizations
- Demonstrates practical Big Data processing techniques

---

## 📁 Project Structure

```text
Large-Scale-Wikipedia-Analytics/
│
├── data/
│   └── wikipedia_sample/
│
├── mapreduce/
│   ├── mapper.py
│   └── reducer.py
│
├── spark/
│   ├── preprocessing.py
│   ├── analysis.py
│   └── queries.py
│
├── notebooks/
│   └── analysis.ipynb
│
├── visualizations/
│   ├── article_growth.png
│   ├── category_distribution.png
│   └── word_frequency.png
│
├── results/
│   └── analysis_results/
│
├── requirements.txt
└── README.md
```

---

## 🚀 Workflow

```text
Download Wikipedia Dump
          ↓
      Store in HDFS
          ↓
    Parse XML Dataset
          ↓
      Clean Data
          ↓
   Hadoop MapReduce
          ↓
     Spark Processing
          ↓
    Statistical Analysis
          ↓
    Visualizations
```

---

## 🧪 Example Analyses

The project can answer questions such as:

- How many articles are present in the dataset?
- Which categories contain the most articles?
- Which words occur most frequently?
- What is the average article length?
- How does Wikipedia content change over time?
- Which knowledge domains show the highest growth?
- How can distributed computing improve processing of Wikipedia-scale datasets?

---

## 📌 Why Big Data Technologies?

Processing the complete Wikipedia dataset using conventional tools such as Pandas on a single machine can become extremely slow and memory-intensive.

Hadoop and Spark overcome this limitation by distributing the workload across multiple processing units.

This makes the project a practical demonstration of:

**Large Dataset → Distributed Storage → Parallel Processing → Analytics → Insights**

---

## 🔮 Outcome

The project demonstrates an end-to-end **Big Data analytics pipeline** capable of processing and analyzing Wikipedia-scale data using distributed computing technologies.

The resulting analysis provides insights into **Wikipedia's article distribution, textual characteristics, knowledge categories, and temporal growth**, while demonstrating the practical application of Hadoop and Spark to a real-world large-scale dataset.
