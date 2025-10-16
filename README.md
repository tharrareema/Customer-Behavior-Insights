 # Customer Behavior Analysis Dashboard

## Overview
This project provides comprehensive analysis of customer behavior patterns, segmentation, and predictive insights using advanced data science techniques.

## Tools Used
- **Python**: Core programming language
- **Pandas**: Data manipulation and analysis
- **Scikit-learn**: Machine learning algorithms (KMeans clustering)
- **Seaborn**: Statistical data visualization
- **Plotly**: Interactive visualizations
- **Jupyter Notebooks**: Interactive analysis environment

## Features

### 1. Customer Segmentation
- **Behavioral Segmentation**: Automatic customer grouping based on behavior patterns
- **KMeans Clustering**: Advanced clustering with optimal cluster selection
- **Segment Analysis**: Detailed insights for each customer segment

### 2. Behavioral Pattern Analysis
- **Purchase Behavior**: Frequency, order value, and lifetime value analysis
- **Engagement Metrics**: Page views, session duration, and interaction patterns
- **Product Preferences**: Category preferences and buying patterns

### 3. Customer Lifetime Value (CLV) Analysis
- **CLV Distribution**: Statistical analysis of customer value
- **High-Value Customer Identification**: Top percentile customer analysis
- **Segment-based CLV**: Value analysis by customer segments

### 4. Engagement Analysis
- **Correlation Analysis**: Relationships between engagement metrics
- **Engagement by Segment**: Segment-specific engagement patterns
- **Behavioral Insights**: Deep dive into customer interaction patterns

### 5. Predictive Insights
- **At-Risk Customer Identification**: Customers likely to churn
- **High-Potential Customers**: Customers with growth potential
- **Actionable Recommendations**: Data-driven business recommendations

## Usage

### Running the Analysis
```bash
cd 02_customer_behavior
python customer_behavior_analysis.py
```

### Key Functions

#### `CustomerBehaviorAnalyzer` Class Methods:
- `generate_sample_data(n_customers=10000)`: Generate synthetic customer data
- `customer_segmentation_analysis()`: Perform KMeans clustering analysis
- `behavioral_patterns_analysis()`: Analyze customer behavior patterns
- `customer_lifetime_value_analysis()`: CLV analysis and visualization
- `engagement_analysis()`: Customer engagement pattern analysis
- `predictive_insights()`: Generate predictive insights and recommendations
- `create_customer_dashboard()`: Create interactive dashboard

## Data Structure

The analysis works with the following customer data structure:
```python
{
    'customer_id': int,
    'age': float,
    'gender': string,
    'income': float,
    'purchase_frequency': int,
    'avg_order_value': float,
    'clv': float,
    'page_views': int,
    'session_duration': float,
    'electronics_preference': float,
    'clothing_preference': float,
    'books_preference': float,
    'satisfaction_score': float,
    'loyalty_score': float,
    'churn_probability': float,
    'customer_segment': string
}
```

## Customer Segments

### 1. Champions
- High CLV and purchase frequency
- Most valuable customers
- Focus: Retention and upselling

### 2. Loyal Customers
- High CLV and loyalty score
- Long-term customers
- Focus: Maintain satisfaction

### 3. Potential Loyalists
- High purchase frequency
- Growing customer base
- Focus: Increase CLV

### 4. New Customers
- Moderate CLV
- Recent acquisitions
- Focus: Onboarding and engagement

### 5. At Risk
- High churn probability
- Declining engagement
- Focus: Retention campaigns

### 6. Need Attention
- Average metrics
- Requires nurturing
- Focus: Engagement improvement

## Key Insights Generated

### 1. Segmentation Insights
- Optimal number of customer clusters
- Cluster characteristics and profiles
- Segment-specific behavior patterns

### 2. Behavioral Insights
- Purchase frequency patterns
- Product preference analysis
- Engagement correlation analysis

### 3. Value Insights
- CLV distribution and statistics
- High-value customer identification
- Segment-based value analysis

### 4. Predictive Insights
- At-risk customer identification
- High-potential customer spotting
- Actionable business recommendations

## Visualizations

### 1. Customer Segments Distribution
- Pie chart showing segment distribution
- Interactive segment exploration

### 2. CLV vs Purchase Frequency
- Scatter plot with satisfaction color coding
- Customer value pattern identification

### 3. Age Distribution by Gender
- Histogram comparison
- Demographic insights

### 4. Product Preferences Heatmap
- Segment-wise preference matrix
- Category preference patterns

### 5. Satisfaction vs Loyalty
- Scatter plot with churn probability
- Customer satisfaction analysis

### 6. Churn Probability by Segment
- Horizontal bar chart
- Risk assessment by segment

## Business Applications

### 1. Marketing Strategy
- Segment-specific campaigns
- Personalized messaging
- Channel optimization

### 2. Customer Retention
- At-risk customer identification
- Retention campaign targeting
- Churn prevention strategies

### 3. Revenue Optimization
- High-value customer focus
- Upselling opportunities
- Cross-selling strategies

### 4. Product Development
- Preference-based recommendations
- Category expansion insights
- Feature prioritization

## Customization Options

### Adding New Metrics
Extend the data structure in `generate_sample_data()`:
```python
'new_metric': np.random.normal(0, 1, n_customers)
```

### Modifying Segments
Update the `_assign_customer_segments()` method with new criteria.

### Adding New Visualizations
Extend the `create_customer_dashboard()` method with additional plots.

## Requirements
- pandas >= 1.5.0
- numpy >= 1.24.0
- matplotlib >= 3.6.0
- seaborn >= 0.12.0
- plotly >= 5.15.0
- scikit-learn >= 1.2.0

## Future Enhancements
- Real-time data integration
- Advanced ML models (RFM analysis)
- A/B testing framework
- Customer journey mapping
- Sentiment analysis integration
