**Case Study: Fast Food - McDonald's Market Segmentation Analysis**

Step 1: Deciding (not) to Segment

The statement is about whether McDonald's should consider market segmentation or not in their marketing strategy.

Step 2: Specifying the Ideal Target Segment

McDonald's management must decide which features make a market segment attractive based on criteria such as homogeneity, distinctiveness, size, matching strengths, identifiability, and reachability. They can focus on solidifying their position in existing segments or understanding and modifying perceptions of segments currently not fond of McDonald's. Liking and frequent consumption of McDonald's are the criteria used in this case study for target segment selection.

Step 3: Collecting Data

The data set contains responses from 1453 Australian consumers about their perceptions of McDonald’s based on 11 attributes and their age and gender. Additional information could have been collected to develop a more detailed market segmentation.

Step 4: Exploring Data

Initial Analysis:

- Imported necessary libraries (NumPy, pandas, matplotlib, seaborn).
- Loaded and examined the dataset, confirming it had 1453 entries and 15 columns, with no missing values.
- Converted categorical responses to binary format (Yes = 1, No = 0) for the first 11 attributes.
- Calculated column means to summarize the average perceptions.
  
Principal Component Analysis (PCA):

- Performed PCA to reduce dimensionality and identify key components.
- The first two components explained significant variance, highlighting key perception differences such as "cheap" vs. "expensive."
  
Step 5: Extracting Segments

K-Means Clustering:

- Explored clustering with K-Means for k values from 2 to 8.
- Determined optimal clusters through the elbow method (inertia vs. number of clusters).
- Visualized results using PCA-transformed data, showing clear segment distinctions.
  
Bootstrap Resampling:

- Repeated clustering with bootstrap samples to assess stability using the Adjusted Rand Index (ARI), providing insights into cluster reliability across different samples.

Gaussian Mixture Models (GMM):

- Applied GMM to fit the data and compare cluster models using BIC and AIC for model selection.
- Plotted BIC and AIC values to determine the optimal number of components, favoring models with lower scores for better fit.
