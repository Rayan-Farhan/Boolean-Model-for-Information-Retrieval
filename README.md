# Boolean Model for Information Retrieval

This project implements a Boolean Information Retrieval model with support for simple and complex Boolean queries, as well as proximity queries. The system uses an inverted index and a positional index to efficiently process queries. A GUI is also provided for user interaction.

## Features

- Text preprocessing using NLTK (tokenization, stemming, stopword removal)
- Inverted index construction for Boolean queries
- Positional index construction for proximity queries
- Boolean query support (AND, OR, NOT)
- Proximity query support with distance operator
- GUI interface built with Tkinter

## How It Works

1. **Preprocessing**:  
   Input text is lowercased, tokenized, stemmed, and filtered for stopwords.

2. **Index Construction**:  
   - `invertedIndex`: Maps terms to documents containing them.  
   - `positionalIndex`: Maps terms to the positions they appear in each document.

3. **Boolean Queries**:  
   - Accepts queries like `"time AND series"` or `"NOT autoencoder"`.
   - Parses and evaluates the Boolean logic.

4. **Proximity Queries**:  
   - Accepts queries like `"feature track /5"`.
   - Finds documents where terms appear within a given distance.

5. **GUI**:  
   A Tkinter-based interface allows users to enter queries without interacting with the code directly.

## Files

- `invertedIndex.txt`: Saved inverted index
- `positionalIndex.txt`: Saved positional index
- `Stopword-List.txt`: List of stopwords
- `./Abstracts/`: Directory containing 448 documents used to build indexes

## Requirements

- NLTK
- pandas
- numpy
- tkinter
