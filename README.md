Internship Recommendation SystemA Machine Learning-based platform designed to bridge the gap between students and career opportunities by matching candidate profiles with relevant internship roles using Natural Language Processing (NLP).
🚀 Overview
  This project implements a recommendation engine that analyzes user skills and candidate data to suggest the best-fitting internships. It utilizes a trained Scikit-Learn model and is deployed via a Python web interface. 
🛠️ Tech StackLanguage: Python  Machine Learning: Scikit-Learn (TF-IDF, Label Encoding, Feature Scaling)  Data Handling: Pandas, NumPy, Pickle  Deployment: Flask / Streamlit (via app.py)  
📂 Project Structureapp.py: 
  The main entry point for the web application.  
  data/: Contains the raw and processed datasets (company.csv, candidate_profile_m...). 
   notebook&data/: Contains the Jupyter Notebook (Model.ipynb) used for training and the exported model artifacts (.pkl files).
     tfidf_vectorizer.pkl: Handles textual feature extraction from descriptions.  scaler.pkl: Ensures numerical data is normalized for the model.  
     internship_recomm...pkl: The finalized trained recommendation model. 
   
⚙️ How It WorksData Processing:
     Candidate profiles and internship descriptions are cleaned and transformed using Label Encoding and TF-IDF Vectorization.  
    Model Training: A recommendation model is trained in the Model.ipynb environment and evaluated for performance.  Inference: When a user enters their skills through app.py, the system scales the input using the saved scaler.pkl and provides the top matches. 
    
🏁 How to RunInstall dependencies: pip install -r requirements.txt
     Run the application: python app.
     pyTips for your individual presentation:Personalization: 
     When discussing this in an interview, emphasize your work in Model.ipynb. Mention that you chose TF-IDF because it allows the system to understand the importance of specific skills rather than just counting words.
      File Clean-up: Before showing this to anyone, remember to delete the files from the Docs folder that reference "Madhan" to maintain the "individual project" narrative.  
