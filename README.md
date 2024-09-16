# Text Summarization Using TextRank

This project demonstrates the use of the TextRank algorithm for text summarization on a dataset of news articles. The goal is to summarize long pieces of text into concise, meaningful summaries using an unsupervised graph-based approach.

## Dataset

The dataset used in this project is a collection of news articles categorized into different topics. It contains two columns:
- `text`: The body of the news article.
- `labels`: The category of the news article (e.g., 'business').

### Sample Data
| text                                                                                                             | labels   |
|------------------------------------------------------------------------------------------------------------------|----------|
| Ad sales boost Time Warner profit. Quarterly profits at US media giant TimeWarner jumped 76%...                   | business |
| BA's profits take off. British Airways' profits have continued their recovery...                                  | business |
| Pernod takeover talk lifts Domecq. Shares in UK drinks and food firm Allied Domecq...                             | business |

The dataset is used to explore how the TextRank algorithm can summarize articles from various topics.

## Project Overview

The project is structured in the form of a Jupyter notebook (`Text_summarization_using_TextRank.ipynb`) and implements the following key steps:

1. **Data Loading and Preprocessing**: Load the dataset and clean the text data for summarization.
2. **TextRank Algorithm**: Implement the TextRank algorithm to rank sentences in an article based on their importance and extract key sentences to form a summary.
3. **Evaluation**: Evaluate the quality of the summaries using ROUGE or other relevant metrics.
4. **Visualization**: Display the original text and the generated summaries to compare the results.

## Installation

To run the notebook, ensure you have the following dependencies installed:

```bash
pip install numpy pandas matplotlib scikit-learn networkx nltk
```

You may also need to download NLTK's stopwords and punkt tokenizer:

```bash
import nltk
nltk.download('stopwords')
nltk.download('punkt')
```

## Usage

To execute the notebook:

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/TextRankSummarization.git
    cd TextRankSummarization
    ```

2. Open the Jupyter notebook:
    ```bash
    jupyter notebook Text_summarization_using_TextRank.ipynb
    ```

3. Run all cells in the notebook to see the summarization process in action.

## Example Output

For a sample news article:
```
Ad sales boost Time Warner profit. Quarterly profits at US media giant TimeWarner jumped 76%...
```

The generated summary might look like:
```
Time Warner reported a significant boost in profits due to high-speed internet sales and ad revenues.
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request to contribute to the project.
