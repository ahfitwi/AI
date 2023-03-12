# Major Steps In Building ML Models
- ML allows the systems to make decisions autonomously without any external support.
- Decisions are made when the machine is able to learn from the data and understand the underlying patterns that are contained within it.
- Through pattern matching and further analysis, they return the outcome which can be a ***classification*** or a ***prediction/regression***.

### 1. Data Collection
  - Collect/garner/gather/glean data applicable to your problem statement you are aspiing to solve using ML Model.
### 2. Data Preprocessing
  - Transform datasets into a form that can be accepted by the ML Models.
  - Scaling/downsampling, Imputation
  - Proprtional and Diversified Data to avoid biases (Alg, data, and societal)
      - If you use 10K images for can and 5K images for dog to create/build a model, it will be biased towards the cat.
  - Create Training, Evaluation, and Testing Sets
### 3. Model Selection
  - Build or select a model that suites your situation
  - Possible Types of Models:
      1. **Supervised Learning**: when there is a precise mapping between input-output data.
          - Dataset, in this case, is labeled, meaning that the algorithm identifies the features explicitly and carries out predictions or classification accordingly.
          - As the training period progresses, the algorithm is able to identify the relationships between the variables/classes such that we can predict a new outcome.

              Input (datasets) + Annotations (tell what each input sets are) --> ML Model --> Prediction
          - Major Supervised Learning Models:
            - **Classification**: response is discrete and belongs to a set of classes. It takes labeled/annotated inputs.
              - Fraud Detection
              - Email Spam Detection
              - Diagnostics
              - Image Classification
            - **Regression/Prediction**: response is continuous
              - Risk Assessment
              - Score Prediction
          - Common Supervised Learning Algorithms:
            - **Linear Regression**: Dependent vs independent vars, where output is continuous and features a constant slope (sales, price)
            - **Random Forest**: used for both classification and regression tasks. Gives output as a class which is the mode or mean of the underlying individual trees.
            - **Gradient Boosting**:sed for both classification and regression tasks. An ensemble of weak prediction models, typically decision trees
            - **Support Vector Machine**: SVMs are powerful classifiers that are used for classifying the binary dataset into two classes with the help of hyperplanes. Effective in cases where a number of dimensions is bigger than the number of samples.
            - **Logistic Regression**: A statistical model that in its basic form uses a logistic function to model a binary variable, although more complex extensions exist.In multivariate analysis , logistic regression (or logit regression) is estimating the parameters of a logistic model (a sort of binary regression).
            - **Artificial Neural Networks(ANN)**: Modeled after the human brain and they learn from the data over time. They form a much larger portion of machine learning called Deep Learning.
            - 
          - Usecases of Supervised Learning:
            - ANN --> Face Recognition
              - CNN is a type of ANN used for identifying the faces of people. Draw/extract features from the image through various filters. Finally, if there is a high similarity score between the input image and the image in the database, a positive match is provided. Baidu has FR in its VSS and expanding to airports, flight check-in.
        
      2. **Unsupervised Learning**:
        - Data is **not explicitly labeled into different classes**, that is, there are no labels. 
        - The model is able to learn from the data by finding implicit patterns.
        - Unsupervised Learning algorithms identify the data based on their densities, structures, similar segments, and other similar features. 
        - Unsupervised Learning Algorithms are based on **Hebbian Learning**.
        - **Cluster analysis** is one of the most widely used techniques in supervised learning.
        - Input (fruits: orange, green peppers, & Apple togehter) --> Model --> Output (clustered: [Green peppers], [Apples], [Oranges])
        - Major Supervised Learning Models:
          - Dimensionality Reduction (SVD/PCA)
            - Text Mining
            - Face Recognition
            - Big Data Visualization
            - Image Recognition
          - Clustering
            - Biology
            - City Planning
            - Targeting Marketing
        - Important algorithms that come under Unsupervised Learning.
          - **Clustering (cluster analysis)** is a technique of grouping similar sets of objects in the same group that is different from the objects in other group.
          - Some of the essential clustering techniques are as follows:
            - **K-Means**: cluster data to k clusters with the nearest mean
          - c
          
        -n
      4. **Reinforcement Learning**: Trial and Error
        - Gaming
        - Finance Sector
        - Manufacturing
        - Inventory Management
        - Robot Navigation
### 4. Model Training
  - 
### 5. Performance Evaluation
  - 
### 6. Performance/Hyperparameter Tunning
  -

# Side Notes:
## Extrapolation:
  - refers to estimating an unknown value based on extending a known sequence of values or facts. To extrapolate is to infer something not explicitly stated from existing information. 
  - refers to predicting values that are outside of a range of data points.
## Interpolation:
  - refers to predicting values that are inside of a range of data points.
  - the act of estimating a value within two known values that exist within a sequence of values.
