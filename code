import streamlit as st
from transformers import pipeline

# Load pre-trained sentiment analysis pipeline
sentiment_analysis = pipeline("sentiment-analysis")

# Streamlit app
st.title("Sentiment Analysis App")

# Input field for the comment
comment = st.text_area("Enter your comment:")

# Run button
if st.button("Analyze Sentiment"):
    if comment:
        # Analyze sentiment
        result = sentiment_analysis(comment)
        # Display result
        st.write("Sentiment Analysis Result:", result)
    else:
        st.write("Please enter a comment to analyze.")
