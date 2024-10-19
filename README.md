# 📰 Fake News Identifier - Machine Learning Project 🧠

This project focuses on identifying fake news using Natural Language Processing (NLP) techniques. The goal is to classify news articles as either **real** or **fake** based on their content.

## 📂 Dataset

We use the [Kaggle Fake News dataset](https://www.kaggle.com/c/fake-news) for this project, which contains the following columns:

- **id**: Unique identifier for each article 🆔
- **title**: The headline or title of the article 📝
- **author**: The author who wrote the article 🖋️
- **text**: The main content of the article 📜
- **label**: The classification label (1 for fake, 0 for real) 🎯

## 🛠️ Technologies Used

- **Python** 🐍
- **TensorFlow** & **Keras** for building the LSTM Model 🤖
- **NLTK** for text preprocessing and tokenization 🛠️
- **Pandas** and **NumPy** for data manipulation 📊
- **Scikit-learn** for evaluation metrics 🧮

## 📚 Workflow

1. **Data Cleaning and Preprocessing**:
   - Removed any missing values in the dataset ✂️
   - Tokenized and stemmed the text using NLTK's `PorterStemmer` ✂️
   - Removed stopwords and applied regex for cleaning 🧽

2. **Model Building**:
   - Used an LSTM (Long Short-Term Memory) neural network to capture the sequence of words 🧬
   - Converted the text into one-hot representations and padded sequences to maintain uniform length 📏
   - Built the model using the following architecture:
     - **Embedding Layer** 🎭
     - **LSTM Layer** 🧠
     - **Dense Layer with Sigmoid Activation** for classification 🖥️

3. **Training and Validation**:
   - Trained the model with **10 epochs** and a **batch size of 64** 🏋️‍♂️
   - Achieved a validation accuracy of **~91%** 📈

4. **Evaluation**:
   - Confusion Matrix 🧮
   - Accuracy Score **~90%** 🔥

## 🔢 Model Summary

| Layer      | Type      | Output Shape      | Param #  |
|------------|-----------|-------------------|----------|
| Embedding  | Embedding | (None, 20, 40)    | 200,000  |
| LSTM       | LSTM      | (None, 100)       | 56,400   |
| Dense      | Dense     | (None, 1)         | 101      |

## 🔥 Performance Metrics

- **Confusion Matrix**:
    ```
    [[3124,  295],
     [ 311, 2305]]
    ```

- **Accuracy**: **89.96%** 🎯

## 🚀 How to Run

1. Clone this repository:

   ```bash
   git clone https://github.com/Gkkumar2/Fake-News-Identifier-ML.git
   ## 🚀 How to Run

2. **Install the necessary dependencies**:

   ```bash
   pip install -r requirements.txt

## 📊 Results and Insights
The model has a high accuracy in detecting fake news, and with further tuning and additional data, it can be improved even more! 🚀

## 🙌 Contributions
Feel free to open a pull request if you'd like to contribute! Any help in improving the dataset, model architecture, or documentation is appreciated. 🛠️

This version organizes the commands properly and removes any extra unnecessary labels, leaving it clear and easy to use. Let me know if you'd like further adjustments! 😊
