## Machine-Learning

My work from studies about programming artificial intelligence on PJATK. This includes such examples as using varius clasification models and trained neural to solve problems like analysis of supermarket customers for marketing purposes or predicting air pollution levels. Originally scripts were developed in google colab using cloud GPU for training neural networks and stored in google drive.

# Neural network with time series

Main topic of this python script is to train neural network to predict level of pollution over city, specifaclly amount of PM2.5 (dust in the air). I used for this air quality data from Wanshou district in Beijing, China, measured from March 2013 to February 2017. 
<img width="1975" height="1063" alt="{AC6B1142-CB41-4F4B-A317-492E6584B311}" src="https://github.com/user-attachments/assets/6e2e7220-4f4b-44f2-98a3-3888f19d515a" />

For that purpose I have prepared time series from initial data, and created small neural network consisting of input, output and three LSTM layers between them. After training, results were quiet satysfying. As we can observe, neural network trained on training data was effective in predicting level of PM2.5 in air.

LSTM neural network

<img width="727" height="269" alt="{92BB67B9-306D-499E-90CF-3E4E288AB91E}" src="https://github.com/user-attachments/assets/067eb67f-27a7-4179-84d4-70146c5aa706" />

Results of predicting
<img width="1614" height="634" alt="image" src="https://github.com/user-attachments/assets/0b845d36-3352-465a-8cb1-f7145517b776" />

Data source file: PRSA_Data_Wanshouxigong_20130301-20170228.csv

# Neural network with encoder-decoder

Main topic of this python script is to distuingish normal from anomalous network traffic, to detect any attack or suspicious activities. This goal will be achieved by training neural network with encoder-decoder architecture. Neural network will be trained on test data with normal traffic. Then, when neural network will try to process data from normal traffic, this operation should be succesfull and have relatively small reconstruction error. Contrary to that, data from abnormal traffic should be rcosntructed with high reconstruction error. In this way, it is possible to predict if network traffic is normal or abnormal.

Many ways of network attack
<img width="202" height="398" alt="{77968EB4-5CD1-4328-A753-7862BAA83966}" src="https://github.com/user-attachments/assets/e9d94063-f1af-4522-bbfa-328be6748639" />

For that purpose neural network with three encoder, and two decoder layers will be used.
<img width="629" height="796" alt="{664BDB36-5116-4116-B4D9-69654228C644}" src="https://github.com/user-attachments/assets/15a98de4-50c1-4087-85b8-64e2b22d1451" />

Results of predicting abnormal network traffic where satisfying, and can be presented with confusion matrix or ROC curve
<img width="484" height="263" alt="{625857C9-AB55-477B-A55E-AEC1B50CB99E}" src="https://github.com/user-attachments/assets/9466cd30-f2b9-4a37-adda-13ecda6fbe8c" />
<img width="691" height="547" alt="image" src="https://github.com/user-attachments/assets/99de0a5a-6c03-4934-b7c5-28c0e318ad62" />

Data source file: https://kdd.ics.uci.edu/databases/kddcup99/kddcup99.html
