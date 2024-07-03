# WhatsApp Chat Analysis

This project involves analyzing a WhatsApp chat using Python, specifically focusing on sentiment analysis of the messages exchanged. The dataset used is in the form of a text file exported from WhatsApp.

## Project Overview

The analysis includes the following steps:

1. **Data Parsing**: Parsing the WhatsApp text file to extract messages along with their timestamps and authors.
2. **Data Cleaning**: Preparing the extracted data for sentiment analysis, ensuring data integrity and completeness.
3. **Sentiment Analysis**: Using NLTK's Vader sentiment analyzer to determine the sentiment scores (positive, negative, neutral) for each message.
4. **Summarizing Sentiments**: Summing up sentiment scores across all messages to derive an overall sentiment for the conversation.

## Tools Used

- **Python Libraries**:
  - `numpy` and `pandas` for data manipulation and analysis.
  - `matplotlib` for visualizations.
  - `re` for regular expressions to parse text.
  - `nltk` for natural language processing tasks, specifically the Vader sentiment analyzer.
  - `wordcloud` for generating word clouds from the messages.
  - `PIL` (Python Imaging Library) for image processing tasks related to word clouds.
  
## File Structure

- **Main Script**: `whatsapp_analysis.py` contains the main code for parsing, analyzing, and summarizing the WhatsApp chat.
- **Data File**: `WhatsApp Chat with Sudeep Pramanik.txt` is the WhatsApp chat exported text file used as input.
- **Output**: Various visualizations (if any) and the sentiment analysis summary are displayed during the script execution.

## Code Explanation

### Parsing WhatsApp Chat

The `whatsapp_analysis.py` script reads the WhatsApp text file line by line, identifying message timestamps and authors using regular expressions (`re`). Messages are then extracted and parsed into a pandas DataFrame.

### Sentiment Analysis

NLTK's Vader sentiment analyzer is applied to each message to compute sentiment scores:
- `Positive`: Positive sentiment score.
- `Negative`: Negative sentiment score.
- `Neutral`: Neutral sentiment score.

These scores are aggregated to determine the predominant sentiment of the conversation.

### Visualization (if included)

If visualization code is present, it generates visual representations of the data, such as plots or word clouds, using `matplotlib` and `wordcloud` libraries.

### Results

The script outputs the sentiment scores for the entire conversation and prints whether the overall sentiment is positive, negative, or neutral based on the sum of scores.

## Running the Script

To run the script:
1. Ensure Python is installed.
2. Install necessary libraries (`numpy`, `pandas`, `matplotlib`, `nltk`, `wordcloud`) if not already installed.
3. Place the WhatsApp chat text file (`WhatsApp Chat with Sudeep Pramanik.txt`) in the same directory as `whatsapp_analysis.py`.
4. Execute `python whatsapp_analysis.py` in your terminal or IDE.

## Conclusion

This project provides insights into the sentiment dynamics of a WhatsApp conversation using basic natural language processing techniques. It serves as a foundational example for more advanced chat analysis and visualization tasks.
