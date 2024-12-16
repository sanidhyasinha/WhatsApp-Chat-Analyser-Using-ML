# WhatsApp Chat Analysis  

Analyze WhatsApp chat data to uncover patterns, trends, and insights into messaging behavior. This project uses Python and its powerful libraries to process and visualize chat statistics, providing actionable insights into group or individual chats.

---

## Table of Contents  

- [Overview](#overview)  
- [Features](#features)  
- [Tech Stack](#tech-stack)  
- [Dataset](#dataset)  
- [Project Structure](#project-structure)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Detailed Analysis](#detailed-analysis)  
- [Sample Outputs](#sample-outputs)  
- [Future Improvements](#future-improvements)  
- [License](#license)  

---

## Overview  

This project analyzes **WhatsApp chat exports** (group or individual conversations) to extract meaningful insights. By applying **data processing** and **visualization techniques**, the project identifies:  

- Most active users  
- Message frequency over time (daily, weekly, monthly trends)  
- Common words used in the conversation  
- Message distribution patterns  
- User behavior statistics  

The project leverages **Python** with libraries like Pandas, Matplotlib, Seaborn, and WordCloud to generate clean and interactive visualizations for easier interpretation.  

---

## Features  

The WhatsApp Chat Analysis project provides the following features:  

1. **Message Statistics**:  
   - Total number of messages  
   - Links shared  
   - Media files sent (e.g., images, videos)  

2. **User Activity Analysis**:  
   - Identify the most active users in a group  
   - Message count per user  

3. **Time-based Trends**:  
   - Daily, weekly, and monthly message frequency  
   - Activity patterns by time of day (morning, afternoon, evening)  

4. **Word Analysis**:  
   - Most common words excluding stopwords  
   - Word Cloud generation for visually appealing representations  

5. **Visualization**:  
   - Generate bar charts, line plots, and word clouds to visualize trends and statistics effectively  

---

## Tech Stack  

- **Programming Language**: Python  
- **Libraries**:  
   - **Pandas**: Data processing and manipulation  
   - **NumPy**: Numerical operations  
   - **Matplotlib** & **Seaborn**: Data visualization  
   - **WordCloud**: Word cloud generation  
   - **Regular Expressions (re)**: Text cleaning and preprocessing  
- **Tools**:  
   - Jupyter Notebook  
   - Git & GitHub  

---

## Dataset  

The project uses **WhatsApp chat export files** (in `.txt` format).  

### How to Export WhatsApp Chat:  
1. Open a chat (individual or group) in WhatsApp.  
2. Go to **Settings > Export Chat**.  
3. Choose **Without Media**.  
4. Save the chat as a `.txt` file.  

Place the file in the `data/` folder of the project directory.  

---

## Project Structure  

The repository follows an organized structure for better readability:  

```
whatsapp-chat-analysis/  
│  
├── data/  
│   ├── chat.txt              # Exported WhatsApp chat file  
│  
├── notebooks/  
│   ├── whatsapp_analysis.ipynb   # Jupyter Notebook with complete analysis  
│  
├── src/  
│   ├── preprocessing.py      # Functions for text cleaning and extraction  
│   ├── analysis.py           # Analysis logic (messages, trends, user stats)  
│  
├── images/  
│   ├── wordcloud.png         # Generated word cloud example  
│   ├── activity_plot.png     # Visualization of activity trends  
│  
├── requirements.txt          # List of dependencies  
├── README.md                 # Project documentation  
└── LICENSE                   # License information  
```

---

## Installation  

To set up and run the project on your local machine:  

### Prerequisites  
- Python 3.8+  
- Jupyter Notebook  

### Steps  

1. **Clone the repository**:  
   ```bash
   git clone https://github.com/campusx-official/whatsapp-chat-analysis.git
   cd whatsapp-chat-analysis
   ```

2. **Create a virtual environment** (optional but recommended):  
   ```bash
   python -m venv venv  
   source venv/bin/activate   # On Windows: venv\Scripts\activate  
   ```

3. **Install required libraries**:  
   ```bash
   pip install -r requirements.txt
   ```

4. **Run Jupyter Notebook**:  
   ```bash
   jupyter notebook
   ```
   Open `notebooks/whatsapp_analysis.ipynb` to perform the analysis.

---

## Usage  

1. Export your WhatsApp chat as a `.txt` file.  
2. Place the file in the `data/` folder as `chat.txt`.  
3. Open the Jupyter Notebook (`notebooks/whatsapp_analysis.ipynb`).  
4. Run all cells to execute the analysis and generate insights.  

---

## Detailed Analysis  

### Preprocessing  
- Clean the raw text using **regular expressions** to extract relevant data (messages, timestamps, users).  
- Filter out media messages, system messages, and stopwords.  

### Analysis Modules  
1. **Message Statistics**: Total messages, media, and links shared.  
2. **User Analysis**: Calculate the number of messages sent by each user and identify the most active participants.  
3. **Time Trends**: Analyze daily, weekly, and monthly trends in message activity.  
4. **Word Frequency**: Extract frequently used words and generate a word cloud visualization.  

### Visualization  
The project generates the following visual outputs:  
- Bar plots for message statistics  
- Line charts for activity trends over time  
- Word clouds for common words  

---

## Sample Outputs  

### 1. Most Active Users  
![Most Active Users](images/activity_plot.png)  

### 2. Word Cloud  
![Word Cloud](images/wordcloud.png)  

### 3. Daily Activity Trends  
Line plots showing message frequency trends by date.  

---

## Future Improvements  

- **Sentiment Analysis**: Classify messages as positive, negative, or neutral using NLP techniques.  
- **Media Analysis**: Include media statistics for chats exported with attachments.  
- **Interactive Dashboards**: Integrate dashboards using Streamlit or Plotly for dynamic visualizations.  
- **Sentiment Timeline**: Analyze user sentiment over time for deeper insights.  
---

## Acknowledgments  

Special thanks to the creators of libraries like **Pandas**, **Matplotlib**, **Seaborn**, and **WordCloud**, which make data analysis and visualization seamless in Python.  
