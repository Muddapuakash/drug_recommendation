# Drug Recommendation System Using DQN and KNN

This project implements an AI-powered drug recommendation system that predicts diseases and suggests suitable drugs, dosages, and precautions based on user symptoms. The system uses a combination of **Deep Q-Network (DQN)** and **K-Nearest Neighbors (KNN)** to learn from user feedback and improve its predictions. 

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [License](#license)

## Project Overview
This project integrates a **DQN model** for drug recommendation, adapting over time based on feedback, and a **KNN model** to classify diseases based on symptoms. The DQN component allows the system to learn optimal drug suggestions, while KNN serves as a baseline for disease classification, assisting in drug selection. The system also considers interactions, efficacy, cost, and patient-specific factors for personalized recommendations.

## Dataset
- The dataset includes symptoms and corresponding diseases, dosages, drug recommendations, and additional considerations for food and allergy interactions.
- Stored as a CSV file (`symptoms_dataset_400_with_dosage.csv`) and preprocessed for compatibility with the DQN and KNN models.

## Features
- **Disease Prediction:** Predict diseases based on symptom inputs using KNN.
- **Drug Recommendation:** Suggest drugs based on user feedback and learned experience using DQN.
- **Interactive UI:** User-friendly interface for inputting symptoms and receiving recommendations.
- **Feedback Learning:** System improves recommendations based on real-time user feedback.
- **Drug Interactions:** Checks for drug-drug, drug-food, and drug-allergy interactions.

## Technologies Used
- **Python**: Core language for developing the model and backend logic.
- **Flask**: Web framework to build the API and serve the UI.
- **Keras**: For building and training the DQN model.
- **Scikit-learn**: For KNN implementation and preprocessing.
- **Pandas**: Data manipulation and handling.
- **JavaScript, HTML, CSS**: Frontend components.

## Setup and Installation
### Prerequisites
- Python 3.7+
- Flask
- Keras
- Scikit-learn
- Pandas

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/Muddapuakash/drug_recommendation.git
   cd drug_recommendation
2. Install dependencies:
    ```bash
   pip install -r requirements.txt
3. Run the Flask app:
   ```bash
   python app.py
Usage
1. Enter symptoms in the input form and click "Get Recommendations.
2. View the predicted disease, suggested drugs, dosages, and precautions.
3. Provide feedback on recommendations to help improve the system.

Project Structure:
   ```bash
            drug_recommendation/
├──  symptoms_dataset_400_with_dosage.csv
├── models/
│   ├── dqn_model.py        # DQN model for drug recommendation
│   ├── knn_model.py        # KNN model for disease prediction
├── templates/
│   ├── index.html          # Frontend HTML template
|   ├── result.html
├── static/
│   └── styles.css          # CSS file for styling
├── app.py                  # Flask app entry point
├── requirements.txt        # Project dependencies
└── README.md               # Project documentation
```
Future Enhancements
Genomic Data Integration: Include pharmacogenomics data for personalized drug recommendations.
Advanced Interactions: Expand drug interaction checks to consider more complex conditions.
Enhanced Visualization: Improve UI and add more detailed visual analytics for user insights.
Contributing
Contributions are welcome! Please create an issue to discuss any changes or improvements you’d like to make. Pull requests are reviewed on a regular basis.

License

   ```bash
### Explanation of Each Section:
- **Project Overview**: Briefly describes the purpose and core functionality.
- **Dataset**: Information about data usage and format.
- **Features**: Key functionalities implemented in the project.
- **Technologies Used**: Lists technologies and libraries.
- **Setup and Installation**: Step-by-step guide for installation and running.
- **Usage**: How to interact with the application.
- **Project Structure**: Overview of the file organization.
- **Future Enhancements**: Potential improvements.
- **Contributing**: How others can contribute.
- **License**: Licensing information.

This structure should make the repository more accessible to users and collaborators. Let me know if you'd like adjustments to any specific sections!
```

