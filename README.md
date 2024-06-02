---

# MyAnswer 🎤

MyAnswer is an innovative web application designed to enhance the viva voce experience for partially blind individuals. Leveraging the power of Vertex AI and generative AI, this app provides a seamless and effective platform for remote examinations and assessments. Teachers can create and manage tests, while students can participate in exams and receive instant feedback through audio and text.

## Team Members
1. [Sandeep Sreekumar](https://github.com/sandeepsreekumar4067)
2. [Nevin](https://github.com/Nevin-10)
3. [Jebin Shaju](https://github.com/jebinshaju)
4. [Aleena Maria Rajesh](https://github.com/prettycoolvariables)

## Link to Product Walkthrough

[Link to video]([Link Here](https://drive.google.com/file/d/1Cw_lX5GIrAEY6QdPkGhvUGthMxq8crkR/view?usp=sharing))

**The site is live at [MyAnswer](https://myanswer-w67ctr3rca-el.a.run.app).**

## How It Works
### Teacher Functionality:
- *Sign Up and Log In*: Teachers can create an account and log in to access the dashboard.
- *Create Tests*: Teachers can create tests by adding questions and answers.
- *Manage Questions*: Teachers can view and manage the questions for each test.
- *View Submissions*: Teachers can view student submissions and check their marks.
- *Generative AI Evaluation*: The app uses generative AI to evaluate student answers and provide detailed feedback.

### Student Functionality:
- *Sign Up and Log In*: Students can create an account and log in to access the dashboard.
- *Enter Examination Code*: Students can enter examination codes to start their exams.
- *Speech-to-Text Answer Capture*: The app uses speech-to-text to capture student answers.
- *Audio Feedback*: Students receive audio feedback on their answers.
- *View Results*: Students can view their previous exam results and receive instant feedback.

## Libraries Used
- Streamlit
- Pyrebase
- Vertex AI
- gTTS (Google Text-to-Speech)
- TemporaryFile
- Base64
- Re
- UUID
- JSON

## Configuration Steps
1. *Clone the Repository*:
    ```bash
    git clone https://github.com/sandeepsreekumar4067/StreamLit_Tinkerhub_2024
    cd myanswer
    ```

2. *Install Required Libraries*:
    ```bash
    pip install -r requirements.txt
    ```

3. *Firebase Configuration*:
    - Set up your Firebase project and configure the firebaseConfig in the app code.
    ```python
    firebaseConfig = {
        'apiKey': "YOUR_API_KEY",
        'authDomain': "YOUR_AUTH_DOMAIN",
        'projectId': "YOUR_PROJECT_ID",
        'storageBucket': "YOUR_STORAGE_BUCKET",
        'messagingSenderId': "YOUR_MESSAGING_SENDER_ID",
        'appId': "YOUR_APP_ID",
        'measurementId': "YOUR_MEASUREMENT_ID",
        'databaseURL': 'YOUR_DATABASE_URL'
    }
    ```

4. *Vertex AI Initialization*:
    - Initialize Vertex AI with your project details.
    ```python
    vertexai.init(project="YOUR_PROJECT_ID", location="YOUR_LOCATION")
    ```

## Running the Application
1. *Run the Streamlit App*:
    ```bash
    streamlit run app.py
    ```

2. *Access the App*:
    - Open your web browser and go to http://localhost:8501.

## Deployment on Google Cloud
1. *Build the Docker Image*:
    ```bash
    docker build -t myanswer .
    ```

2. *Push the Docker Image to Google Container Registry*:
    ```bash
    docker tag myanswer gcr.io/your-project-id/myanswer
    docker push gcr.io/your-project-id/myanswer
    ```

3. *Deploy to Cloud Run*:
    ```bash
    gcloud run deploy myanswer --image gcr.io/your-project-id/myanswer --platform managed
    ```

## Key Features
- *Accessibility*: Enhances the viva experience for partially blind students with audio-based interactions.
- *Generative AI*: Utilizes Vertex AI for evaluating student answers and generating detailed, explanatory feedback.
- *Instant Feedback*: Provides immediate feedback and results to students, making the learning process more efficient.
- *User-Friendly*: Simple and intuitive interface for both teachers and students, ensuring a seamless user experience.

## Conclusion
MyAnswer revolutionizes the viva voce process for partially blind individuals by integrating advanced AI technologies to create an inclusive, effective, and user-friendly examination platform. Join us in making education more accessible and engaging for everyone.



---
