# YouTube-Analytics-Optimizing-Video-Performance-with-PySpark

## Overview
This project analyzes YouTube trending videos data to uncover insights about video performance, engagement patterns, and optimal posting strategies. Using PySpark for large-scale data processing, the project examines factors that contribute to a video's success, including posting times, content categories, metadata features, and engagement metrics.

## Dataset
- Contains trending video data with views, likes, comments, and metadata.
- Includes publish date, trending date, and category info.
- Used to analyze engagement patterns and optimal posting strategies.
- Limited to trending videos only (survivorship bias).
- Download here: https://drive.google.com/file/d/1sv9nXXWf9YUisAMH7XIpzX-oyfFF-sPQ/view?usp=drive_link
## Key Features

### 1. Data Cleaning and Preparation
- Converts raw timestamp strings to proper datetime formats
- Handles null values in numerical columns
- Calculates days between video publication and trending
- Extracts publishing hour and day of week
- Parses video tags and calculates tag counts
- Creates engagement scores based on likes, comments, and views
- Maps category IDs to human-readable names

### 2. Analytical Components

#### Best Times to Post Analysis
- Identifies optimal days of the week for posting
- Determines best hours of the day for maximum visibility
- Analyzes average time between posting and trending

#### Content Insights
- Examines performance across different video categories
- Analyzes impact of tag usage on engagement
- Studies title length characteristics of trending videos

#### Regional Differences
- Compares trending patterns across different channels
- Identifies channel-specific optimal posting times
- Analyzes category preferences by channel

#### Engagement Patterns
- Studies what drives comments and likes
- Calculates like-to-view and comment-to-view ratios by category
- Examines how tag count affects engagement

### 3. Visualization
Generates visualizations for:
- Average views by day of week
- Average views by hour of day
- Performance across video categories
- Engagement patterns by tag count

### 4. Recommendations
Produces data-backed recommendations for content creators including:
- Best days and times to post
- Most successful content categories
- Optimal tag usage and title length
- Engagement optimization strategies

## Technical Implementation
- Built with PySpark for distributed data processing
- Uses Spark SQL for complex aggregations and transformations
- Implements window functions for advanced analytics
- Generates visualizations with matplotlib
- Outputs results to CSV for further analysis

## Usage
1. Ensure PySpark is installed and configured
2. Update the dataset path in the code
3. Run the analysis notebook
4. Review generated:
   - Visualizations
   - CSV output files
   - Recommendations text file

## Output Files
- `day_analysis.csv`: Performance metrics by day of week
- `hour_analysis.csv`: Performance metrics by hour of day
- `category_analysis.csv`: Performance by video category
- `country_analysis.csv`: Performance by channel
- `country_category_analysis.csv`: Category preferences by channel
- `youtube_recommendations.txt`: Actionable insights for creators

## Dependencies
- PySpark
- pandas
- matplotlib
- Python 3.x

This analysis provides valuable insights for content creators looking to optimize their YouTube strategy and for analysts studying video performance patterns on the platform.
