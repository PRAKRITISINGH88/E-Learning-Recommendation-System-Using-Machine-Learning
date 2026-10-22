# E-Learning Recommendation System Using Machine Learning

An intelligent course recommendation platform designed to help learners discover relevant online courses based on their interests, skills, and learning preferences using Machine Learning and Natural Language Processing (NLP).

## 📌 Project Overview

The **E-Learning Recommendation System Using Machine Learning** aims to make online learning more personalized and efficient. With thousands of courses available across different platforms, learners often find it difficult to identify courses that match their interests, current skills, and career objectives.

This project uses machine learning and text similarity techniques to recommend relevant courses based on course descriptions, topics, and other available course information.

The project is developed as a final-year B.Tech Computer Science and Engineering capstone project with a specialization in Data Science.

## 🎯 Objectives

- Recommend relevant online courses based on learner interests.
- Apply Machine Learning and NLP techniques to course recommendation.
- Process and analyze course-related datasets.
- Improve course discovery through content similarity.
- Develop a user-friendly web application for exploring recommendations.
- Provide a foundation for future career-oriented learning recommendations.

## ✨ Key Features

- **Course Search:** Search courses using keywords and topics.
- **Personalized Course Discovery:** Discover courses similar to a selected course.
- **Content-Based Filtering:** Use course information to identify relevant learning resources.
- **Text Processing:** Process course descriptions and related text using NLP techniques.
- **Similarity-Based Ranking:** Rank courses according to their content similarity.
- **Interactive Web Interface:** Explore course information and recommendations through a web application.
- **Scalable Design:** Provide a foundation for adding more advanced recommendation methods.

> Note: Features such as learner-profile personalization, career-path recommendations, and skill-gap analysis are planned enhancements unless they have been implemented in the current version.

## 🛠️ Technology Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Backend | Flask |
| Machine Learning | Scikit-learn |
| Data Processing | Pandas, NumPy |
| Natural Language Processing | TF-IDF |
| Recommendation Technique | Content-Based Filtering |
| Similarity Measure | Cosine Similarity |
| Frontend | HTML, CSS, JavaScript |
| Testing | pytest, Playwright |

## 🧠 Machine Learning Methodology

The recommendation workflow consists of the following stages:

1. **Data Collection:** Load the course dataset containing available course information.
2. **Data Preprocessing:** Clean course text and prepare relevant fields for analysis.
3. **Feature Extraction:** Apply TF-IDF vectorization to represent textual course information numerically.
4. **Similarity Calculation:** Calculate cosine similarity between course representations.
5. **Recommendation Ranking:** Identify and rank courses with similar content.
6. **Result Presentation:** Display recommended courses through the web application.

### Recommendation Workflow

```text
Course Dataset
      |
      v
Data Preprocessing
      |
      v
Text Feature Extraction (TF-IDF)
      |
      v
Course Similarity Calculation
      |
      v
Recommendation Ranking
      |
      v
Recommended Courses
      |
      v
Web Application
```

## 📂 Project Structure

```text
e-learning-recommendation-system-ml/
│
├── app.py                 # Flask web application
├── model.py               # Model generation and recommendation logic
├── requirements.txt       # Python dependencies
├── requirements-dev.txt   # Development and testing dependencies
│
├── data/
│   └── cleaned_dataset.csv
│
├── models/                # Generated model artifacts
│
├── templates/
│   └── index.html         # Web application interface
│
├── static/
│   ├── css/
│   │   └── styles.css
│   └── js/
│       └── script.js
│
├── tests/                 # Automated tests
├── .gitignore
├── LICENSE
└── README.md
```

*The exact file and folder names may vary depending on your final implementation.*

## 💻 Installation and Setup

### Prerequisites

Install the following software before running the project:

- Python 3.12 (recommended for dependency compatibility)
- Visual Studio Code or another Python IDE
- Git
- A modern web browser

### Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/e-learning-recommendation-system-ml.git
```

Replace `YOUR_USERNAME` with your GitHub username.

### Step 2: Navigate to the Project Directory

```bash
cd e-learning-recommendation-system-ml
```

### Step 3: Create a Virtual Environment

On Windows:

```powershell
py -3.12 -m venv .venv
```

Activate the environment:

```powershell
.\.venv\Scripts\Activate.ps1
```

If PowerShell blocks activation, run the following command in the current terminal and activate the environment again:

```powershell
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
.\.venv\Scripts\Activate.ps1
```

### Step 4: Install Dependencies

Upgrade pip:

```bash
python -m pip install --upgrade pip
```

Install project dependencies:

```bash
pip install -r requirements.txt
```

For development and testing:

```bash
pip install -r requirements-dev.txt
```

### Step 5: Generate Model Files

If the required precomputed model files are missing, run:

```bash
python model.py
```

This step generates the model artifacts required by the application. It may take some time depending on your system.

### Step 6: Run the Application

```bash
python app.py
```

### Step 7: Open the Application

Open the following URL in your browser:

```text
http://127.0.0.1:5000/
```

The application should now be available locally.

To stop the server, press `Ctrl + C` in the terminal.

## 📊 Dataset

The project uses a course dataset containing information about online courses.

Depending on the available columns, the dataset may include:

- Course titles
- Course descriptions
- Course categories
- Course difficulty levels
- Course ratings
- Skills associated with courses
- Course provider information
- Course URLs

**Dataset reference:** [Coursera Course Dataset on Kaggle](https://www.kaggle.com/datasets/siddharthm1698/coursera-course-dataset)

Review the dataset's license and usage terms before redistributing it with your repository.

## 📈 Evaluation

The recommendation system should be evaluated using suitable measures to understand the quality and relevance of its recommendations.

Potential evaluation measures include:

- **Precision@K:** Measures how many of the top K recommendations are relevant.
- **Recall@K:** Measures how many relevant courses appear among the top K recommendations.
- **NDCG@K:** Measures the quality of the ranking, accounting for the positions of relevant courses.
- **Response Time:** Measures the time needed to generate recommendations.

These metrics require suitable relevance labels, user feedback, or an appropriate evaluation dataset. Results should be reported only after running the evaluation.

## 🚀 Future Enhancements

The following features can extend the project into a more advanced learning recommendation platform:

1. **Learner Profile:** Collect current skills, interests, and learning preferences.
2. **Career-Based Recommendations:** Recommend courses for roles such as Data Scientist, Data Analyst, and Machine Learning Engineer.
3. **Skill-Gap Analysis:** Compare existing learner skills with skills required for a selected career.
4. **Hybrid Recommendation Engine:** Combine content-based recommendations with collaborative filtering when sufficient interaction data is available.
5. **Learning Path Generation:** Arrange recommended courses in a logical learning sequence.
6. **Interactive Analytics Dashboard:** Use Power BI to analyze course categories, ratings, difficulty levels, and skill demand.
7. **Recommendation Evaluation:** Compare algorithms using appropriate ranking metrics.
8. **Deployment:** Deploy the application to a suitable cloud platform.

## 🎓 Academic Information

**Project Title:** E-Learning Recommendation System Using Machine Learning

**Degree:** Bachelor of Technology (B.Tech)

**Department:** Computer Science and Engineering

**Specialization:** Data Science

**Project Type:** Final-Year Capstone Project

**Team Members:** Add the names of your project team members here.

**Institution:** Add your university name here.

## 👥 Team Contributions

Update this section with the actual responsibilities of each team member.

| Team Member | Responsibility |
|---|---|
| Member 1 | Data collection and preprocessing |
| Member 2 | Machine learning and recommendation algorithms |
| Member 3 | NLP and feature engineering |
| Member 4 | Backend development and API integration |
| Member 5 | Frontend development and user interface |
| Member 6 | Testing, evaluation, and analytics dashboard |

## 📚 Learning Outcomes

Through this project, the team aims to gain practical experience in:

- Data preprocessing and exploratory data analysis
- Machine Learning and recommendation systems
- Natural Language Processing
- Feature extraction and similarity measures
- Web application development using Flask
- Software testing and model evaluation
- Git and GitHub-based collaboration

## 🔐 License and Attribution

This repository may incorporate or adapt code from existing open-source projects. Retain applicable copyright notices, licenses, and attribution when reusing such code.

If this implementation is adapted from the original Course Recommendation System by Samuel Aboye, acknowledge the source:

[Original Course Recommendation System](https://github.com/saboye/Course-Recommendation-System)

Review the original project's license and the dataset's separate terms before distributing the adapted implementation.

## 📬 Contact

For questions, feedback, or collaboration, contact:

**Project Maintainer:** PRAKRITI SINGH

**GitHub:** https://github.com/PRAKRITISINGH88
---

⭐ If you find this project useful, consider starring the repository.

*Developed as a final-year Data Science capstone project focused on machine learning-based course discovery and recommendation.*
