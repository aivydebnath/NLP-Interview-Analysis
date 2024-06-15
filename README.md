# Interviewing Candidates with Data Science Experience from Diverse Backgrounds 

## Overview
As part of the hiring process for a specialized data science role within our organization, interviewed candidates with varying backgrounds across different domains. Yet, all share significant experience in data science. The objective was to assess their qualifications and suitability for the specific requirements of the role.

## Context:
In our pursuit to fill a critical data science position, candidates with a proven track record in data analysis, machine learning, and statistical modeling. Recognizing the interdisciplinary nature of data science, we welcomed applicants from diverse fields such as:

Finance
Healthcare
Engineering
Marketing
Academia
Insurance
Automotive
Entertainment
Real Estate

## Data:

The dataset interview.txt contains the details of 30 candidates who gave the interview and their responses.

## Approach:

I have used TextBlob for sentiment analysis and Spacy for keyphrase extraction.

1. Reading the Transcript:

            The read_interview_responses function reads the entire content of a text file containing the interview responses and returns it as a single string.

            Splitting and Processing Responses: The process_interview_responses function splits the transcript into individual responses using a regular expression. Each response is then further processed to extract the candidate information and their detailed response.
   
2. Sentiment Analysis:

            The analyze_sentiment function uses TextBlob to determine the sentiment of each candidate's response.

         It classifies the sentiment as "Positive," "Negative," or       "Neutral," and assigns a corresponding sentiment score (1 for positive, -1 for negative, 0 for neutral).

3. Key Phrase Extraction:

            The extract_key_phrases function uses spaCy to extract key phrases (noun chunks) from each response. These key phrases are then converted to lowercase for            consistency.
   
4. Quality Assessment:

            The script evaluates the relevance of key phrases by comparing extracted phrases to a predefined set of relevant key phrases related to data science and    
       machine learning.
               The relevance score is calculated as the proportion of relevant key phrases found in the response.

            An overall quality score is computed by combining the sentiment score and the relevance score.
   
            Based on the quality score, each response is classified into one of four categories: "Excellent," "Good," "Fair," or "Poor".

## Output:

The results showed a candidate number, the response the candidate has given, the sentiment of the response, key phrases used by the candidates, and Relevant key phrases that pull out the words relevant to the DS role we are offering, and at the last Overall quality of the assessment as per the transcripted.
