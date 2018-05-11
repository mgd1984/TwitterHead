### TwitterHead

TwitterHead is an IoT prototype digital art project. It visualizes tweets according to their sentiment score by flashing different coloured LEDs inside a clear glass skull. The patterns of flashing lights are intended to symbolize the firing of neurons inside the human brain.

#### Background 
As a kid, I used to love taking apart old toys, figuring out how they worked, and hacking together new contraptions from their innards.  Perhaps it was 'Back to the Future' or 'Honey, I Shrunk the Kids', but I definitely developed an appreciate for the eccentric creator types that created mind-blowing technology. Although we don't have time-travelling Delorians or shrink ray-guns (that I am aware of), some of the tech we get to play around with in the 21st Century still seems like magic to me sometimes.    

![Back to the Future](https://cdn.quizzclub.com/trivia/2017-11/what-is-doc-allergic-to-in-the-movie-back-to-the-future.jpg)
![Honey, I Shrunk the Kids](https://vignette.wikia.nocookie.net/disney/images/3/34/Shrink_Ray_2.jpg/revision/latest?cb=20140112183317)

Having worked with tech startups, entrepreneurs and incubators for many years, I came to be familiar with some of the tools that they used to develop prototypes and projects. In particular, I was attracted to a few hardware prototyping platforms - Arduino and more recently, Raspberry Pi. These hardware hacking platforms are perfect for developing prototypes and proof-of-concept designs for various projects like IoT, home automation, wearables, etc. Combined with some coding and data science, you can do some pretty cool things, relatively simply.  

### Installation & Config

###

###

### Node-Red Flow for 'TwitterHead' IoT Application
1. Configure & Connect to Twitter Node (authorize app & set node to listen for keywords, hashtages, or users)
2. Sentiment Node passes Msg to Switch Node which routes the Msg based on it's 'sentiment.score' value. 
3. Connect Switch Node to Trigger Nodes to send 1 (ON) or 0 (OFF) to Raspberry Pi GPIO Pinout Node(s).
4. Connect the Trigger Nodes to Raspberry Pi GPIO Pinout Nodes to fire the 'neurons' (LEDs) in the TwitterHead.
5. Send Msg.payload to Debug Node to diagnose any errors.   

![TwitterHead Node Red](https://storage.googleapis.com/oa-video-test-bucket/Screen%20Shot%202018-05-09%20at%202.48.58%20PM.jpg)

![TwitterHead](https://storage.googleapis.com/oa-video-test-bucket/IMG_38B31954FCE3-1.jpeg)
![TwitterHead Electronics](https://storage.googleapis.com/oa-video-test-bucket/IMG_1827.PNG)


#### Testing the Setup 
[![TwitterHead](https://storage.googleapis.com/oa-video-test-bucket/Screen%20Shot%202018-05-09%20at%2011.30.25%20PM.jpg)](https://youtu.be/HNA7sXDd9Sg "TwitterHead")

