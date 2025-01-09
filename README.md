# Nextword_predection
A custom on-screen keyboard application built with Python and Tkinter, featuring dynamic text display and word suggestions. 
This project implements a word prediction module using trigram analysis. It predicts the next likely words based on a given word by analyzing a provided corpus of text. The project utilizes the NLTK library for natural language processing and pandas for data handling.

Features   
Predicts the next three likely words based on the input word.    
Uses trigram analysis to determine word probabilities.    
Processes a text corpus (all_data.txt) to build a model for predictions.    
Provides a fallback mechanism when no matches are found.    

How It Works    
Input: The user provides a word (new_text) as input.  
Corpus Analysis: The script reads a text corpus (all_data.txt) to extract trigrams.  
Trigram Analysis: It finds the most frequent word combinations where the input word is the first word.  
Prediction: It suggests up to three likely words based on frequency and context.  

Limitations  
Predictions are based only on the provided corpus. Larger and more diverse corpora improve accuracy.
Handles only English text.  
May return the input word if no match is found in the corpus.  
