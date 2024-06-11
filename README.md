>>Hate Speech Analyzer
  This project is a simple Hate Speech Analyzer built using Python, tkinter for the GUI, and scikit-learn for text classification. 
  The application uses a Logistic Regression model trained on a dataset of tweets to classify input text as either "Hate Speech" or "Not Hate Speech".

>>Table of Contents
  ->Overview
  ->Features
  ->Installation
  ->Usage
  ->How It Works
  ->Dataset
  ->Model Training
  ->GUI Implementation
  ->License

>>Overview
  The Hate Speech Analyzer allows users to input a text message and determine whether it is hate speech or not.
  It utilizes a pre-trained Logistic Regression model for the classification task. The user interface is implemented using tkinter,a standard Python interface to the Tk GUI toolkit.

>>Features
  Text Classification: Classifies text as either "Hate Speech" or "Not Hate Speech".
  Graphical User Interface: Easy-to-use GUI for text input and result display.
  Model Training and Testing: Includes steps for training the model and testing its accuracy.

>>Installation
  To set up and run this project, follow the steps below:

>>Prerequisites
  Ensure you have the following installed on your machine:
    ->Python 3.x
    ->pip (Python package installer)
    ->Clone the Repository
    ->Clone this repository to your local machine using the following command:
    ->pandas
    ->scikit-learn
    ->tkinter
    Note: tkinter is included in the standard Python library, so you might not need to install it separately.

>>Prepare the Dataset
  Ensure you have a CSV file named hateSpeech_dataset.csv in the project directory. The CSV file should have the following structure:
  tweet	class
  Your tweet text here...	0 or 1
  tweet: The text of the tweet.
  class: 0 for "Not Hate Speech", 1 for "Hate Speech".

>>Usage
  To run the Hate Speech Analyzer, navigate to the project directory and execute the script:
  python hate_speech_analyzer.py
  This will launch the application window where you can input text and analyze it for hate speech.

>>User Interface
  Enter Text: Type or paste the text you want to analyze in the provided text box.
  Analyze Button: Click the "Analyze" button to classify the text.
  Result Display: The classification result will be displayed in a new window.
  
>>How It Works
  ->Dataset
    The dataset used for training is a collection of tweets with labels indicating whether each tweet is "Hate Speech" or "Not Hate Speech". The dataset is loaded into a pandas DataFrame for preprocessing.

>>Model Training
  Load and Split Data: The dataset is split into training and testing sets using train_test_split.
  Text Vectorization: The text data is transformed into numerical vectors using TfidfVectorizer, which converts the text into a matrix of TF-IDF features.
  Model Training: A Logistic Regression model is trained on the vectorized text data. The model is configured with a maximum of 1000 iterations to ensure convergence.
  Model Evaluation: The trained model is evaluated on the test set, and its accuracy and classification report are printed to the console.
  GUI Implementation
  The GUI is implemented using tkinter and includes the following components:

>>Main Window:
  The root window is created with a title and specified dimensions.
  Canvas and Frame: A canvas is used as a background, and a frame is placed on it to hold the text box and buttons.
  Text Input: A Text widget allows users to enter or paste text for analysis.
  Analyze Button: A button triggers the analyze_text function, which processes the input text and displays the result in a new window.
  Result Window: A new window shows the input text and the classification result ("Hate Speech" or "Not Hate Speech").
  The analyze_text function retrieves the text from the input box, processes it through the predict_hate_speech function, and displays the result.

Feel free to contribute to this project by submitting issues or pull requests. Your feedback is highly appreciated!

>>Example Screenshot:

  ->When text is hate speech:
    <img width="732" alt="Screenshot 2024-06-12 at 1 06 06 AM" src="https://github.com/RahimAbbas55/Hate-Speech-Analyzer-using-Logistic-Regression-Model/assets/101935846/8456a166-f223-4a2c-a63a-522dc0b82cf2">

  ->When text is not hate speech:
    <img width="729" alt="Screenshot 2024-06-12 at 1 06 36 AM" src="https://github.com/RahimAbbas55/Hate-Speech-Analyzer-using-Logistic-Regression-Model/assets/101935846/28896af4-3512-475d-bf25-384e65b769bc">

  ->Model Accuracy and Classification Report:
    <img width="491" alt="Screenshot 2024-06-12 at 1 08 10 AM" src="https://github.com/RahimAbbas55/Hate-Speech-Analyzer-using-Logistic-Regression-Model/assets/101935846/c63eaf0c-e282-49c3-a6d3-921fe23b315d">





