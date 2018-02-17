# G-ClsReg-Kaiser-Perez
regression + classification project

### a) 
Matthew Kaiser and Robert Perez

### b)
Use the Myo band to send data to wekinator to train regression model which can tell how hard you hard flexing your arm.

### c)
For our project we used the MYO gesture armband, Processing, Wekinator and some online pictures for our output.

### d)
We used a second degree polynomial regression algorithm in our project because, if you try to picture it, the data that is being fed in needs to increase in probability around where it should be, climax at a certain point, and then go back down as the probability of the next increases. Our project tests how much someone is flexing across eight channels of eeg data so there need to be bands of probability that increase and decrease in their separate ranges. We chose not to do linear because that didn’t fit the data, and the neural net took far longer to train for no noticeable improvement in performance.

### e)
Our Wekinator model is trained using the second degree polynomial regression algorithm to send out a range for a classifaiction program written in Processing to classify the strength of an arm flex producing a picture as a result to show the streangth in a range of 1 to 3.

### f)
One of the technical challenges I tried to solve but couldn’t was AWT input event implementation in processing which didn’t work at all to try to simulate mouse clicks to allow you to play skyrim with the myoband. Another technical challenge was figuring out how to catch each of the eight parts of data, average them over time, and then send them to wekinator so the data wasn’t so volatile. I did this by writing a smoothing array five deep that would take the average of the absolute value over each individual channel and then output that. There was also another function that updated the array each time new data arrived.

### g)
https://www.youtube.com/watch?v=VVsuWsejmic&feature=youtu.be

### h)
In completing this project we learned how to interface a Myo armband with processing and wekinator to classify how hard a user is flexing their arm.  We also learned about optimal ways to smooth data such that the high frequency of data recieved from the Myo armband may be smoothed for a more accurate classification. 
