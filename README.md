TOPSIS-Based Ranking of Pre-Trained Conversational Models
Overview
This project utilizes the TOPSIS (Technique for Order Preference by Similarity to Ideal Solution) method to systematically rank pre-trained conversational AI models based on multiple performance criteria.

Dataset & Models
The following five pre-trained models are evaluated:

GPT-3.5
T5
XLNet
BERT
DialoGPT
Each model is assessed using the following criteria:

Accuracy (Higher is better)
Perplexity (Lower is better)
Response Time (Lower is better)
BLEU Score (Higher is better)
F1 Score (Higher is better)
Methodology
Normalization: Min-Max scaling is used to standardize values.
Weight Assignment: Each criterion is weighted based on significance.
TOPSIS Calculation:
Compute ideal best and ideal worst values.
Determine Euclidean distances from ideal values.
Compute TOPSIS scores to rank models.
Installation & Usage
Prerequisites
Ensure Python and the following dependencies are installed:

bash
Copy
Edit
pip install numpy pandas matplotlib scikit-learn seaborn
Execution
Run the script to compute model rankings and generate visualizations.

Results
The output ranks models based on TOPSIS scores. The final rankings are as follows:

Model	TOPSIS Score	Rank
GPT-3.5	0.679623	1
T5	0.657469	2
XLNet	0.404832	3
BERT	0.362986	4
DialoGPT	0.320377	5


Visualization Outputs
📊 Bar Chart: Comparison of TOPSIS scores across models.
🥧 Pie Chart: Score distribution breakdown.
🔥 Heatmap: Weighted normalized decision matrix visualization.
Contributions
Feel free to contribute by:

Adding new pre-trained models
Modifying evaluation criteria
Optimizing the TOPSIS calculation