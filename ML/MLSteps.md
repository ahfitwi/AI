# Major Steps In Building ML Models
- ML allows the systems to make decisions autonomously without any external support.
- Decisions are made when the machine is able to learn from the data and understand the underlying patterns that are contained within it.
- Through pattern matching and further analysis, they return the outcome which can be a ***classification*** or a ***prediction/regression***.
- ML Model <-- [Data, Algorithm, Training]
- There is a science about how to build an ML.

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
          - Input (datasets) + Annotations (tell what each input sets are) --> ML Model --> Prediction
          -  Algorithm consists of a target/outcome variable (or dependent variable) which is to be predicted from a given set of predictors (independent variables).
          -  Training continues until the model acieves the desired level of accuracy on the training data.
          - Major Supervised Learning Models:
            - **Classification**: response is discrete and belongs to a set of classes. It takes labeled/annotated inputs.
              - Fraud Detection
              - Email Spam Detection
              - Diagnostics
              - Image Classification
            - **Regression/Prediction**: response is continuous (Predictors vs Depenednet Vars)
              - Risk Assessment
              - Score Prediction
          - Common Supervised Learning Algorithms:
            - **Linear Regression**: Dependent vs independent vars, where output is continuous and features a constant slope (sales, price)
            - **Random Forest**: used for both classification and regression tasks. Gives output as a class which is the mode or mean of the underlying individual trees.
            - **Gradient Boosting**:sed for both classification and regression tasks. An ensemble of weak prediction models, typically decision trees
            - **Support Vector Machine**: SVMs are powerful classifiers that are used for classifying the binary dataset into two classes with the help of hyperplanes. Effective in cases where a number of dimensions is bigger than the number of samples.
            - **Logistic Regression**: A statistical model that in its basic form uses a logistic function to model a binary variable, although more complex extensions exist.In multivariate analysis , logistic regression (or logit regression) is estimating the parameters of a logistic model (a sort of binary regression).
            - **Artificial Neural Networks(ANN)**: Modeled after the human brain and they learn from the data over time. They form a much larger portion of machine learning called Deep Learning.
          - Usecases of Supervised Learning:
            - ANN --> Face Recognition
              - CNN is a type of ANN used for identifying the faces of people. Draw/extract features from the image through various filters. Finally, if there is a high similarity score between the input image and the image in the database, a positive match is provided. Baidu has FR in its VSS and expanding to airports, flight check-in.
        
      2. **Unsupervised Learning**:
        - Data is **not explicitly labeled into different classes**, that is, there are no labels. 
        - No target or outcome variable to predict/estimate (w/c is called unlabelled data)
        - The model is able to learn from the data by finding implicit patterns.
        - Unsupervised Learning algorithms identify the data based on their densities, structures, similar segments, and other similar features. 
        - Unsupervised Learning Algorithms are based on **Hebbian Learning**.
        - **Cluster analysis** is one of the most widely used techniques in supervised learning.
        - Input (fruits: orange, green peppers, & Apple togehter) --> Model --> Output (clustered: [Green peppers], [Apples], [Oranges])
        - Draw inferences/patterns from input w/o references to labeledd outcomes.
        - Major Supervised Learning Models:
          - Dimensionality Reduction (SVD/PCA: reduce dimensions of feature sets and are of two types, namely feature elimination or feature extraction)
            - Text Mining
            - Face Recognition
            - Big Data Visualization
            - Image Recognition
          - Clustering (customer segmentation, Fraud Detection, & Document Classification)
            - Biology
            - City Planning
            - Targeting Marketing
        - Important algorithms that come under Unsupervised Learning.
          - **Clustering (cluster analysis)** is a technique of grouping similar sets of objects in the same group that is different from the objects in other group. Some of the essential clustering techniques are as follows:
            - **K-Means**: cluster data to k clusters with the nearest mean.
            - **DBSCAN**: groups the data based on the density. It groups together the points that are given in the space and marks the outliers in the low-density region.
            - **Hierarchical clustering**: In this form of clustering, a hierarchy of clusters is built.
            - **Anomaly Detection**: these techniques detect outliers in the unlabeled data under an assumption that most of the data examples are normal by observing the instances that fit the remainder of the data set.
            - **Autoencoders**: A type of Neural Networks that are used in Unsupervised Learning for representation learning. They are used in denoising and dimensionality reduction.
            - **Deep Belief Network**: It is a generative graphical model which is also a class of neural network designed for unsupervised learning. It is different from the supervised type of neural networks in the sense that it probabilistically reconstructs its inputs to act as feature detectors.
            - **Principal Component Analysis**: It is a class of unsupervised learning paradigm which is used for reducing the dimensions of the data.
        - **Unsupervised Learning Use Case**: One of the most popular unsupervised learning techniques is **clustering**. Using clustering, businesses are able to capture potential customer segments for selling their products.
          - Sales companies are able to identify customer segments that are most likely to use their services. Companies can evaluate the customer segments and then decide to sell their product to maximize the profits.
          - One such company that is performing brand marketing analytics using Machine Learning is an Israeli based startup – Optimove. The goal of this company is to ingest and process the customer data in order to make it accessible to the marketers.
          - They take it one step further by providing smart insights to the marketing team, allowing them to reap the maximum profit out of their product marketing.
          - Used for recommendation systems or clustering (segments customers into d/t groups for specific interventions)
      4. **Reinforcement Learning**: Trial and Error
        - covers more area of Artificial Intelligence which allows machines to interact with their dynamic environment in order to reach their goals. With this, machines and software agents are able to evaluate the ideal behavior in a specific context.
        - With the help of this reward feedback, agents are able to learn the behavior and improve it in the longer run. This simple feedback reward is known as a reinforcement signal.
        - The agent in the environment is required to take actions that are based on the current state. This type of learning is different from Supervised Learning in the sense that the training data in the former has output mapping provided such that the model is capable of learning the correct answer. Whereas, in the case of reinforcement learning, there is no answer key provided to the agent when they have to perform a particular task. When there is no training dataset, it learns from its own experience.
        - Reinforcement Learning Use Case:
          - Google’s Active Query Answering (AQA) system makes use of reinforcement learning.It reformulates the questions asked by the user.
          - For example, if you ask the AQA bot the question – “What is the birth date of Nikola Tesla” then the bot would reformulate it into different questions like “What is the birth year of Nikola Tesla”, “When was Tesla born?” and “When is Tesla’s birthday”.
          - This process of reformulation utilized the traditional sequence2sequence model, but Google has integrated reinforcement Learning into its system to better interact with the query based environment system.
          - This is a deviation from the traditional seq2seq model such that all the tasks are carried out using reinforcement learning and policy gradient methods. That is, for a given question q0, we want to obtain the best possible answer a*.
          - The goal is to maximize the award $a* = argmaxa R(ajq0)$.
          - Others:
            - Gaming
            - Finance Sector
            - Manufacturing
            - Inventory Management
            - Robot Navigation
### 4. Model Training
  - Pass the training dataset into the model so that the model will be able to extract features, calculate weights, and understand what they are.
### 5. Performance Evaluation
  - Test how accurate the model can classifyor predict the test data
### 6. Performance/Hyperparameter Tunning
  - Trial and Error Step: Tune the number of Nodes, Functions, Filters, ...
  - Usually model construction is iterative
### 7. Do Prediction: 
  - Start Using the Model to predict new real-world data
## Summary
Concluding the article, I took a look at the common steps of ML model creation/construction/building from data collection through hyperparameter tuning, and different types of machine learning paradigms. I went through supervised, unsupervised and reinforcement learning algorithms. I also discussed the several common algorithms that are part of these three categories accompanied by their various real-life applications.

# Side Notes:
## Extrapolation:
  - refers to estimating an unknown value based on extending a known sequence of values or facts. To extrapolate is to infer something not explicitly stated from existing information. 
  - refers to predicting values that are outside of a range of data points.
## Interpolation:
  - refers to predicting values that are inside of a range of data points.
  - the act of estimating a value within two known values that exist within a sequence of values.

## Types of Customer Segmentations (8)
  - Demographic (Age, Gender, Income, Education, Social Status, Family, Life Stage, Occupation)
  - Geographic (country, city, Density, Language, Climate, Area, Population)
  - Behavioral (Benefits Sought, Purchase, Usage, Intent, Occasion, Buyer Stage, User Stattus, Life Cycle Stage, Engagement)
  - Value-based
  - Needs-based
  - Technographic
  - Psychographic (Lifestyle, AIO, Concerns, Personality, Value, Attitudes)
  - Life Cycle Stage
## Customer Classification
  - Loyal
  - Fan
  - Supporter
  - Roamers
##
