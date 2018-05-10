# TwitterHead
#### Node-Red Flow for 'TwitterHead' IoT Application

1. Configure & Connect to Twitter Node (authorize app & set node to listen for keywords, hashtages, or users)
2. Sentiment Node passes Msg to Switch Node which routes the Msg based on it's 'sentiment.score' value. 
3. Connect Switch Node to Trigger Nodes to send 1 (ON) or 0 (OFF) to Raspberry Pi GPIO Pinout Node(s).
4. Connect the Trigger Nodes to Raspberry Pi GPIO Pinout Nodes to fire the 'neurons' (LEDs) in the TwitterHead.
5. Send Msg.payload to Debug Node to diagnose any errors.   

![TwitterHead Node Red](https://storage.googleapis.com/oa-video-test-bucket/Screen%20Shot%202018-05-09%20at%202.48.58%20PM.jpg)

![TwitterHead](https://storage.googleapis.com/oa-video-test-bucket/IMG_38B31954FCE3-1.jpeg)

[![TwitterHead](https://storage.googleapis.com/oa-video-test-bucket/Screen%20Shot%202018-05-09%20at%2011.30.25%20PM.jpg)](https://youtu.be/HNA7sXDd9Sg "TwitterHead")
