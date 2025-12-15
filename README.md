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
