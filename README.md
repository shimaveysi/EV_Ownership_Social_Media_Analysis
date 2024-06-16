Web and Social Media Analytics for Electric Vehicles
Introduction
This project focuses on analyzing discussions around Fully Electric Vehicles (FEVs) using social media data. FEVs are chosen for their significant impact on reducing carbon emissions and their growing popularity. The project aims to understand industry trends, identify key discussion themes, and analyze sentiments towards FEVs.
Industry Overview
The electric vehicle (EV) industry is rapidly expanding, driven by technological advancements, government incentives, and increasing consumer awareness about environmental issues. Key trends include:
•	Battery Technology Advancements: Improvements in battery technology are enhancing range, efficiency, and affordability.
•	Government Incentives: Tax credits, rebates, and grants are encouraging EV adoption.
•	Charging Infrastructure Expansion: Investments in fast-charging networks and renewable energy integration are critical.
•	Autonomous Driving: EVs are often at the forefront of autonomous driving technology.
Prominent EV Models
1.	Tesla Model 3:
o	Range: Up to 353 miles (Long Range version)
o	Features: Autopilot, over-the-air updates, minimalist interior
o	Market Position: Known for strong performance and advanced technology
2.	Nissan Leaf:
o	Range: Up to 226 miles (Leaf Plus version)
o	Features: ProPILOT Assist, e-Pedal, spacious interior
o	Market Position: Best-selling for its practicality and value
Data Collection and Preprocessing
Keywords and Search Terms
We focused on keywords related to FEVs such as "fully electric vehicle", "Tesla Model 3", "Nissan Leaf", "EV charging", and "electric car range".
Data Collection Method
Reddit was chosen for its diverse and active communities discussing EVs. We used Reddit's API to collect posts with relevant keywords, achieving a total dataset size between 500 and 2000 posts.
Preprocessing Steps
•	Duplicate Removal: Ensured each post is unique.
•	Missing Values Handling: Removed entries with missing text fields.
•	Text Cleaning: Replaced newline characters with spaces.
•	Timestamp Conversion: Converted Unix timestamps to human-readable formats.
Sample Code for Data Collection
python
Copy code
# Step 1: Install necessary libraries
!pip install praw nest_asyncio

# Step 2: Import Libraries and Set Up Reddit API Credentials
import praw
import nest_asyncio
nest_asyncio.apply()

# Step 3: Define Keywords and Collect Data
keywords = ["fully electric vehicle", "Tesla Model 3", "Nissan Leaf"]
# ... (additional code to collect data)

# Step 4: Preprocessing the Data
# ... (additional code for preprocessing)
Exploratory Analysis
Popular Words and Phrases
Frequent terms include "car", "electric", "vehicle", "tesla", "model", and "charging".
Word Associations and Correlations
Common bigrams are "model 3", "electric vehicle", "nissan leaf", "tesla model", and "electric car".
Time-Series Analysis
Analyzed the number of posts over time to identify peaks corresponding to significant industry events.
Visualizations
•	Word Frequency: Bar charts of most frequent words.
•	Bigram Frequency: Bar charts of common word pairs.
•	Time-Series: Line plots of post counts over time.
Text Mining
Topic Modeling
Used Latent Dirichlet Allocation (LDA) to identify discussion themes:
•	General Car Discussions
•	Nissan Leaf Specific
•	EV Range and Battery Life
•	Charging Infrastructure
•	Tesla Model 3 Specific
Sentiment Analysis
Used VADER for sentiment analysis, categorizing posts as:
•	Neutral: 311 posts
•	Positive: 275 posts
•	Negative: 168 posts
Evaluation Metrics
•	Coherence Score: 0.316 (moderate, indicating reasonable topic coherence)
•	Sentiment Analysis Metrics: Precision, recall, and F1-score all at 1.00 (suggesting high accuracy but potential overfitting)
Conclusion
Our analysis of EV discussions on social media reveals key themes and sentiments, providing valuable insights for stakeholders. Common concerns include charging infrastructure and battery range. Future work should expand data sources and refine modeling techniques to capture a broader range of perspectives and improve model coherence.
Recommendations
•	Address Charging Infrastructure and Battery Concerns: Enhance reliability and accessibility.
•	Broaden Data Collection: Include diverse social media platforms.
•	Explore Advanced Modeling Techniques: Improve topic coherence and sentiment analysis accuracy.
