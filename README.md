# Deep Learning(CSED538/AIGS538) Final Project, FedWAGG(Federated Learning based on Weighted Aggregation)

This project proposes a federated learning methodology, FedWAGG using weighted clustering method to solve the non-I.I.D issue of federated learning.
We confirmed FedWAGG has a stabilizing effect for the learning of global model on Non-I.I.D datasets in federated learning.

## Environment Configuration
Recommended Environment
`Python 3.8 or 3.9`
`x86_64 Linux` \
We do not require GPUs to run the assignments.

## How to Run
Make sure you already installed python with recommended versions above.

Using ipynb\
Run FEDWAGG.ipynb file. \
In Jupyter Notebook, you can use run `Run All` cells

Using python script\
pip install -r requirements.txt\
python FedWAGG.py

## Project Information
Number of clients: 9
Number of clients per cluster: 3
Model: 2-Layer Convolutional Neural Network

Training data:
	Num of Training set: 1500
	Num of Test set: 200
	client_data_distributions:
		1 (default): 
			[0.45, 0.45, 0.03, 0.01, 0.01, 0.01, 0.01, 0.01, 0.01, 0.01],
			[0.01, 0.45, 0.45, 0.03, 0.01, 0.01, 0.01, 0.01, 0.01, 0.01],
			[0.01, 0.01, 0.45, 0.45, 0.03, 0.01, 0.01, 0.01, 0.01, 0.01],
			[0.01, 0.01, 0.01, 0.45, 0.45, 0.03, 0.01, 0.01, 0.01, 0.01],
			[0.01, 0.01, 0.01, 0.01, 0.45, 0.45, 0.03, 0.01, 0.01, 0.01],
			[0.01, 0.01, 0.01, 0.01, 0.01, 0.45, 0.45, 0.03, 0.01, 0.01],
			[0.01, 0.01, 0.01, 0.01, 0.01, 0.01, 0.45, 0.45, 0.03, 0.01],
			[0.01, 0.01, 0.01, 0.01, 0.01, 0.01, 0.01, 0.45, 0.45, 0.03],
			[0.03, 0.01, 0.01, 0.01, 0.01, 0.01, 0.01, 0.01, 0.45, 0.45],
		2: 
		    	[0.9, 0.02, 0.01, 0.01, 0.01, 0.01, 0.01, 0.01, 0.01, 0.01],
			[0.01, 0.9, 0.02, 0.01, 0.01, 0.01, 0.01, 0.01, 0.01, 0.01],
			[0.01, 0.01, 0.9, 0.02, 0.01, 0.01, 0.01, 0.01, 0.01, 0.01],
			[0.01, 0.01, 0.01, 0.9, 0.02, 0.01, 0.01, 0.01, 0.01, 0.01],
			[0.01, 0.01, 0.01, 0.01, 0.9, 0.02, 0.01, 0.01, 0.01, 0.01],
			[0.01, 0.01, 0.01, 0.01, 0.01, 0.9, 0.02, 0.01, 0.01, 0.01],
			[0.01, 0.01, 0.01, 0.01, 0.01, 0.01, 0.9, 0.02, 0.01, 0.01],
			[0.01, 0.01, 0.01, 0.01, 0.01, 0.01, 0.01, 0.9, 0.02, 0.01],
			[0.01, 0.01, 0.01, 0.01, 0.01, 0.01, 0.01, 0.01, 0.9, 0.02],

## Results
Short summary)
Summarizing our experimental results, FEDWAGG had the effect of stabilizing global model learning. However, there was no significant performance improvement in FEDWAGG compared to FEDAVG for non-IID dataset.
Please refer [final report](https://github.com/junsoo37/FedWAGG/blob/master/FEDWAGG_report.pdf) to check full results.

<img width="800" alt="image" src="https://github.com/junsoo37/FedWAGG/assets/73781220/f239cef3-5a80-4f5d-b9bd-605b934c59a6">

Team with
  - Sumin Song (songsm921@postech.ac.kr)
  - Chanyoung Maeng (mcy5712@postech.ac.kr)
