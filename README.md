# 🍽️ EazyDiner Restaurant Analysis

> A comprehensive data science project analyzing 1,591+ restaurants in Bengaluru using web scraping, data processing, and advanced analytics. Key findings demonstrate that restaurant success is not solely dependent on premium pricing, with budget-friendly establishments often matching or exceeding premium restaurant ratings.

---

## 📋 Table of Contents

- [Overview](#overview)
- [Project Highlights](#project-highlights)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Data Processing Pipeline](#data-processing-pipeline)
- [Key Insights](#key-insights)
- [Installation & Usage](#installation--usage)
- [Features Engineered](#features-engineered)
- [Visualizations](#visualizations)
- [Business Recommendations](#business-recommendations)
- [Future Enhancements](#future-enhancements)

---

## 🎯 Overview

This end-to-end data science project demonstrates a complete workflow for restaurant market analysis:

- **Data Collection**: Web scraping 1,200+ restaurants from EazyDiner Bengaluru
- **Data Cleaning**: Comprehensive data validation and quality assurance
- **Exploratory Data Analysis (EDA)**: Statistical and categorical analysis
- **Feature Engineering**: 11 derived features for deeper insights
- **Visualization**: Interactive dashboards and compelling charts
- **Business Intelligence**: Actionable recommendations for stakeholders

---

## ⭐ Project Highlights

| Feature | Description |
|---------|-------------|
| **1,200+ Restaurants** | Comprehensive dataset from Bengaluru |
| **Data Cleaning Pipeline** | Validation and quality assurance on 1,591 records after processing |
| **11 Engineered Features** | Derived metrics for personalized scoring and segmentation |
| **Parametric Value Scoring** | Custom recommendation function based on price/rating balance |
| **Regional Analysis** | Insights across 5+ geographic regions of Bengaluru |
| **Cuisine Segmentation** | 25+ cuisine types analyzed and categorized |
| **Advanced Visualizations** | Compelling charts for regional, categorical, and numerical analysis |

---

## 🛠️ Tech Stack

### Programming & Data Processing
```
✓ Python 3.x        - Core programming language
✓ Pandas             - Data manipulation & analysis
✓ NumPy              - Numerical computations
✓ Beautiful Soup     - Web scraping
✓ Regular Expressions - Text pattern matching & cleaning
```

### Data Visualization & Storage
```
✓ Matplotlib         - Statistical visualizations
✓ Seaborn            - Advanced plotting
✓ CSV Files          - Data storage
✓ Jupyter Notebook   - Interactive development environment
```

---

## 📁 Project Structure

```
EazyDiner-Restaurant-Analysis/
├── notebooks/
│   ├── 01_data_scraping.ipynb              # Web scraping & collection
│   ├── 02_data_cleaning.ipynb              # Data validation & preprocessing
│   ├── 03_exploratory_data_analysis.ipynb  # Statistical & visual analysis
│   └── 04_feature_engineering.ipynb        # Feature creation & scoring
│
├── data/
│   ├── raw_restaurants.csv                 # Scraped dataset (raw)
│   ├── cleaned_restaurants.csv             # Processed dataset (cleaned)
│   └── analysis_results.csv                # Analysis outputs
│
├── visualizations/
│   ├── regional_analysis.png
│   ├── price_distribution.png
│   ├── cuisine_heatmap.png
│   └── value_scoring_insights.png
│
├── README.md                               # This file
└── requirements.txt                        # Project dependencies
```

---

## 🔄 Data Processing Pipeline

### Phase 1: Data Collection
- Scraped restaurant data from EazyDiner Bengaluru
- Extracted attributes: name, cuisine, ratings, price, location, category
- Handled pagination and dynamic content

### Phase 2: Data Cleaning
- **Removed duplicates** and invalid records
- **Standardized formats** across text fields
- **Handled missing values** intelligently
- **Validated data types** for numerical fields
- **Final dataset**: 1,591 restaurants with 1.7% loss rate

### Phase 3: Exploratory Analysis
- **Univariate analysis**: Distribution of prices, ratings, and cuisines
- **Bivariate analysis**: Relationships between features
- **Regional segmentation**: Market dynamics across Bengaluru zones
- **Statistical testing**: Identifying significant patterns

### Phase 4: Feature Engineering
Created 11 derived features:
- **Value Score**: Rating-to-price ratio for value assessment
- **Price Percentile**: Restaurant's position in price distribution
- **Cuisine Diversity**: Multiple cuisine offerings
- **Rating Categories**: Binned ratings for segmentation
- **Regional Metrics**: Zone-specific benchmarks
- ...and 6 more contextual features

---

## 💡 Key Insights

### Market Structure
```
Budget Segment (<₹1,000)     : 38% of restaurants
Mid-range Segment (₹1,000-3,000) : 43% of restaurants
Premium Segment (>₹3,000)    : 19% of restaurants
```

### Pricing Dynamics
| Region | Avg Cost | Count | Strategy |
|--------|----------|-------|----------|
| **South Bengaluru** | ₹905 | 922 | Budget-friendly, High volume |
| **West Bengaluru** | ₹962 | 52 | Premium focus, Low density |
| **North Bengaluru** | ₹925 | 202 | Moderate pricing |
| **East Bengaluru** | ₹908 | 209 | Balanced approach |
| **Central Bengaluru** | ₹901 | 161 | Mixed positioning |

### Rating Analysis
- **Average Rating**: 3.8/5 with standard deviation of 0.6
- **Highest Rated Cuisines**: North Indian, Continental
- **Most Common Rating Range**: 3.5-4.0 (40% of restaurants)
- **Premium restaurants** don't necessarily have higher ratings

### Cuisine Preferences
- **Top 5 Cuisines**: North Indian, Chinese, Continental, Cafe, South Indian
- **Specialty restaurants** often command premium prices with niche customer base
- **Multi-cuisine venues** dominate the mid-range segment

---

## 🚀 Installation & Usage

### Prerequisites
```bash
Python 3.8+
pip (Python package manager)
```

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/Vasanth4321/EazyDiner-Restaurant-Analysis.git
   cd EazyDiner-Restaurant-Analysis
   ```

2. **Create virtual environment** (optional but recommended)
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

5. **Navigate through notebooks** in this order:
   - `01_data_scraping.ipynb`
   - `02_data_cleaning.ipynb`
   - `03_exploratory_data_analysis.ipynb`
   - `04_feature_engineering.ipynb`

---

## 🔧 Features Engineered

### Quantitative Features
- **Value Index**: `Rating / (Price / 1000)` - measures value delivery
- **Price Percentile**: Restaurant's ranking in price distribution
- **Rating Tier**: Categorical binning of numerical ratings
- **Cuisine Versatility**: Count of cuisine offerings

### Categorical Features
- **Price Segment**: Budget/Mid-range/Premium classification
- **Region Zone**: Geographic segmentation
- **Cuisine Category**: Primary cuisine classification
- **Rating Level**: Excellent/Good/Average/Below Average

### Derived Metrics
- **Regional Benchmarks**: Zone-specific averages
- **Competitive Positioning**: Against regional peers
- **Recommendation Score**: Parametric scoring function

---

## 📊 Visualizations

Key charts generated during analysis:

1. **Price Distribution** - Histogram showing market segmentation
2. **Rating vs Price Scatter** - Identifying value leaders
3. **Regional Heatmap** - Geographic price patterns
4. **Cuisine Distribution** - Top cuisines and frequency
5. **Value Score Comparison** - Restaurant recommendation ranking
6. **Cumulative Distribution** - Market concentration analysis

---

## 🎯 Business Recommendations

### For New Restaurant Operators
- **Entry Strategy**: Budget segment offers high volume but intense competition
- **Differentiation**: Focus on unique cuisines or superior ratings at competitive prices
- **Regional Choice**: South Bengaluru offers volume; Premium areas (West) offer margin

### For Investors
- **Market Trends**: Mid-range segment (₹1,000-3,000) shows balanced opportunity
- **Quality Focus**: Ratings matter more than pricing in customer retention
- **Expansion**: South Bengaluru shows highest restaurant density with growth potential

### For Food Delivery Platforms
- **Onboarding Priority**: Multi-cuisine restaurants in mid-range segment
- **Marketing Focus**: Value-scoring restaurants for promotional campaigns
- **Commission Strategy**: Tier-based approach reflecting value delivery

---

## 📈 Project Status: COMPLETE WITH ACTIONABLE INSIGHTS

✅ Data Collection: 1,200+ restaurants analyzed  
✅ Data Cleaning: 1,591 records after processing  
✅ Feature Engineering: 11 derived features created  
✅ Value Scoring: Parametric function developed  
✅ Visualizations: Compelling regional & categorical charts  
✅ Business Insights: Comprehensive recommendations for stakeholders  

---

## 🔮 Future Enhancements

- [ ] **Sentiment Analysis**: Restaurant reviews text mining
- [ ] **Predictive Modeling**: ML models for rating/price prediction
- [ ] **Dynamic Dashboard**: Interactive Tableau/Power BI dashboard
- [ ] **Temporal Analysis**: Seasonal trends and growth patterns
- [ ] **Image Analysis**: Restaurant ambiance classification
- [ ] **API Integration**: Real-time data updates from EazyDiner
- [ ] **Recommendation System**: Personalized restaurant suggestions

---

## 🤝 Contributing

This is a personal portfolio project, but suggestions and feedback are welcome! Feel free to:
- Open issues for bugs or improvements
- Submit pull requests with enhancements
- Share ideas for additional analysis

---

## 👨‍💻 Author

**Vasanth** - Aspiring Data Scientist & Analyst  
📍 Hyderabad, Telangana, India  
🔗 [GitHub Profile](https://github.com/Vasanth4321) | [Portfolio](https://github.com/Vasanth4321?tab=repositories)

---

## 🙏 Acknowledgments

- EazyDiner for the restaurant data source
- Data science community for best practices

---

## 📞 Questions or Feedback?

Feel free to reach out via GitHub Issues or contact through my profile. I'm always interested in discussing data science projects and insights!
