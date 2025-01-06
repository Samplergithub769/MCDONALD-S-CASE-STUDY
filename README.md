**Case Study: Fast Food - McDonald's Market Segmentation Analysis**

Step 1: Deciding (not) to Segment

Discussion: Whether McDonald's should implement market segmentation in its marketing strategy. This decision hinges on whether segmentation can better address diverse customer needs or if a more uniform approach would suffice.

Step 2: Specifying the Ideal Target Segment

Criteria: McDonald’s management evaluates segments based on:
- Homogeneity
- Distinctiveness
- Size
- Alignment with company strengths
- Identifiability
- Reachability
Focus: Determine which segments favor McDonald's and which do not, aiming to enhance positive perceptions or address negative ones.

Step 3: Collecting Data

Dataset: Responses from 1453 Australian consumers were gathered on 11 perception attributes, along with age and gender data.

Analysis Foundation: Data collection aimed at segmenting the market based on consumer perceptions.

Step 4: Exploring Data

Initial Analysis:

- Imported necessary libraries (NumPy, pandas, matplotlib, seaborn).
- Loaded and examined the dataset, confirming it had 1453 entries and 15 columns, with no missing values.
- Converted categorical responses to binary format (Yes = 1, No = 0) for the first 11 attributes.
- Calculated column means to summarize the average perceptions.
Principal Component Analysis (PCA):

- Performed PCA to reduce dimensionality and identify key components.
- The first two components explained significant variance, highlighting key perception differences such as "cheap" vs. "expensive."
- 
Step 5: Extracting Segments

K-Means Clustering:

- Explored clustering with K-Means for k values from 2 to 8.
- Determined optimal clusters through the elbow method (inertia vs. number of clusters).
- Visualized results using PCA-transformed data, showing clear segment distinctions.
- 
Bootstrap Resampling:

- Repeated clustering with bootstrap samples to assess stability using the Adjusted Rand Index (ARI), providing insights into cluster reliability across different samples.
- 
  Gaussian Mixture Models (GMM):

- Applied GMM to fit the data and compare cluster models using BIC and AIC for model selection.
- Plotted BIC and AIC values to determine the optimal number of components, favoring models with lower scores for better fit.
