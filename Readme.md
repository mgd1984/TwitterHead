# TwitterHead
#### Node-Red Flow for 'TwitterHead' IoT Application

1. Configure & Connect to Twitter Node (authorize app & set node to listen for keywords, hashtages, or users)
2. Sentiment Node passes Msg to Switch Node which routes the Msg based on it's 'sentiment.score' value. 
3. Connect Switch Node to Trigger Nodes to send 1 (ON) or 0 (OFF) to Raspberry Pi GPIO Pinout Node(s).
4. Connect the Trigger Nodes to Raspberry Pi GPIO Pinout Nodes to fire the 'neurons' (LEDs) in the TwitterHead.
5. Send Msg.payload to Debug Node to diagnose any errors.   

![TwitterHead Node Red](https://lh3.googleusercontent.com/yZdqDQpK2iLAxqz9po7Cwptcl_BYAi3PZai7UJe1eyyRIbr2BMQw6oQQ09DFSTXjOjRS9OSfFqMZbjcO2M_F=w1440-h717-rw)

![TwitterHead](https://lh5.googleusercontent.com/8j3UisTcgjk0T1K515lADWHs99bnxBzH7mSgxJ1U1PXCoXCg1KWhz0y6akHo8wszVvAXoo7WPZSumkk4AFic=w1440-h717-rw)
