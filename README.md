# Search Ranking Model — LambdaMART

A Learning-to-Rank system that ranks search results intelligently, 
similar to how Google Search works.

## Results
| Method | NDCG@10 |
|--------|---------|
| BM25 Baseline | 0.257 |
| LambdaMART | 0.465 |
| **Improvement** | **+81%** |

## Dataset
- MSLR-WEB10K by Microsoft
- 723K query-document pairs
- 136 features per document
- Relevance labels 0-4

## What This Does
- Loads real search ranking dataset
- Computes BM25 baseline score
- Trains LambdaMART model using LightGBM
- Evaluates using NDCG@10 metric
- Plots feature importance
- Shows before/after ranking demo

## Tech Stack
- Python
- LightGBM (LambdaMART)
- Pandas, NumPy
- Matplotlib

## Key Concept
BM25 puts 5 irrelevant results in top 10.  
LambdaMART puts 9 relevant results in top 10.
