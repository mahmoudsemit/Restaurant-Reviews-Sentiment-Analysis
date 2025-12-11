Restaurant Reviews Dataset – Using NLTK + TextBlob
________________________________________
1. Introduction
This report presents a comprehensive sentiment analysis of a dataset containing restaurant reviews. The goal is to:
•	Clean and preprocess text using NLTK-style text normalization
•	Apply stemming using the PorterStemmer
•	Remove stopwords
•	Analyze sentiment using TextBlob Polarity Scores
•	Classify each review into Positive, Negative, or Neutral
•	Extract insights about customer perception
•	Provide recommendations to improve business performance
________________________________________
2. Data Overview
The dataset consists of text reviews provided by restaurant customers. These reviews vary in tone from highly positive praise to complaints about food quality and service.
Each review was processed through a pipeline involving:
1.	Lowercasing
2.	Tokenization
3.	Stopword removal
4.	Punctuation removal
5.	Porter stemming
6.	Sentiment scoring with TextBlob
________________________________________
3. Preprocessing Summary
A custom preprocessing pipeline was applied:
•	Stopword Removal: Common English words that do not carry meaning (e.g., “the”, “is”, “and”) were removed.
•	Punctuation Removal: All punctuation such as '.', '!', ',' was stripped.
•	Stemming: Words were reduced to their root form (e.g., “loved” → “love”, “tasty” → “tasti”).
•	TextBlob Polarity: Each cleaned review was assigned a polarity score between –1.0 
________________________________________
4. Sentiment Classification Method
Sentiment was labeled based on polarity:
•	Polarity > 0 → Positive
•	Polarity < 0 → Negative
•	Polarity = 0 → Neutral
This allows a simple and interpretable division of reviews.
________________________________________
5. Sentiment Distribution
After running analysis:
Overall Breakdown
•	Positive reviews: The majority of customers expressed satisfaction, praising food quality, pricing, menu variety, and atmosphere.
•	Negative reviews: A smaller portion complained about taste, service delays, rude staff, or poor food texture.
•	Neutral reviews: Mostly factual comments without emotional charge.
________________________________________
6. Key Insights from Positive Reviews
Positive reviews commonly include:
•	Taste & Quality: “delicious”, “amazing”, “loved”, “fresh”, “great flavor”
•	Service: “friendly staff”, “quick service”, “welcoming”
•	Atmosphere: “cozy”, “nice ambiance”
•	Value: “good price”, “worth the money”
This indicates customers strongly appreciate:
✔ Good flavor
✔ Friendly service
✔ Menu variety
✔ Competitive pricing
________________________________________
7. Key Insights from Negative Reviews
Negative reviews mostly revolve around:
•	Bad taste or texture: “nasty”, “not tasty”, “overcooked”
•	Poor service experience: “slow”, “rude”, “ignored”
•	Price dissatisfaction: “overpriced”, “not worth it”
•	Food inconsistency: good one visit, poor another
Customers are most sensitive to:
⚠ Long waiting times
⚠ Rude or inattentive staff
⚠ Low-quality food compared to expectations
________________________________________
8. Neutral Reviews Themes
Neutral reviews tend to be:
•	Simple observations (“Stopped by during holiday…”)
•	Factual statements about menu items
•	Reviews lacking emotional words
These provide context but do not indicate strong satisfaction or dissatisfaction.
________________________________________
9. Limitations
Every sentiment analysis method has limitations:
1.	Negation Handling: Stem-based methods can misinterpret sentences like
“not good” → interpreted as positive after stemming
2.	Sarcasm: TextBlob cannot detect sarcastic comments
3.	Context Loss: Stemming removes nuance (e.g., “tasty” → “tasti”)
4.	Terse Reviews: Very short reviews may default to neutral
A more advanced model (e.g., VADER or transformer-based) improves accuracy.
________________________________________
10. Business Recommendations
Based on sentiments extracted:
✔ Enhance Training for Staff
Negative reviews frequently mention slow or rude service. Improving service consistency can significantly raise overall satisfaction.
✔ Improve Food Consistency
Several negative comments addressed inconsistent taste. Standardizing recipes can reduce complaints.
✔ Monitor Pricing Perception
A minority mentioned “overpriced”. Review pricing strategy relative to competitors.
✔ Leverage Positive Feedback
Many customers praise:
•	Flavor
•	Menu variety
•	Ambiance
•	Staff friendliness
Highlight these strengths in marketing campaigns.
✔ Collect More Feedback
Encourage customers to leave reviews to increase dataset size and sentiment diversity.
________________________________________
11. Conclusion
The sentiment analysis reveals that the restaurant maintains a strong positive customer perception overall, with most reviews highlighting quality food and good service. However, notable negative sentiment focuses on service delays and inconsistent taste, areas that the business can target for improvement.

