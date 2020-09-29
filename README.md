# Distributed-system-for-specific-people-detection
This system is composed of three elements:
the first entity intended to analyze the video received in order to find the person sought.
The third entity is a broker for the exchange of data.
The third entity receives the data which are the name of the person found, the timestamp and his location.
We put the photo of the person that we need to find in the folder 'Basic Images'. 
When the person is detected we save his name, timestamp and his location in a the csv folder 'data.csv' 
then we send those datas to the broker on the 'tracking' topic in order that the third entity which is subscribred on the same topic get also the datas.
