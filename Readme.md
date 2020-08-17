### TwitterHead

TwitterHead is an IoT prototype digital art project. It visualizes tweets according to their sentiment score by flashing different colour LEDs inside a clear glass skull. The patterns of flashing lights are intended to symbolize the firing of neurons inside the human brain.

#### Background 
As a kid, I used to love taking apart old toys, figuring out how they worked, and hacking together new contraptions from their innards.  Perhaps it was 'Back to the Future' or 'Honey, I Shrunk the Kids', but I definitely developed an appreciation for the eccentric creator types that created mind-blowing technology. Although we don't have time-travelling Delorians or shrink ray-guns (that I am aware of), some of the tech we get to play around with in the 21st Century still seems like magic to me sometimes.    

![Back to the Future](https://cdn.quizzclub.com/trivia/2017-11/what-is-doc-allergic-to-in-the-movie-back-to-the-future.jpg)
![Honey, I Shrunk the Kids](https://vignette.wikia.nocookie.net/disney/images/3/34/Shrink_Ray_2.jpg/revision/latest?cb=20140112183317)

Having worked with in incubators and with tech startups for many years, I came to be familiar with the tools used by designers, developers, and inventors of prototypes and technology projects. In particular, I was attracted to hardware prototyping platforms such as Arduino and Raspberry Pi. These hardware hacking platforms are perfect for developing prototypes and proof-of-concept designs for various projects such as Internet of Things, home automation, wearables, and many others. Combined with some coding, data science, and creativity, you can do some pretty cool things.  

### Installations & Setup

**Tools Used** 

***Hardware***
* 1x Raspberry Pi Zero (W)
* 1x Micro-USB Charger
* 4x Copper Wire LED Strips 
* Jumper Cables 

***Software/Libraries/Packages/Apps***
* Node-RED - a virual flow-based development tool for wiring IoT applications originally developed by IBM, written in Javascript. 
* Node Package Manager - package manager for Javascript 
* Node.js - JavaScript run-time environment that executes JavaScript code server-side [Wikipedia](https://en.wikipedia.org/wiki/Node.js)
* 

###

### Node-Red Flow for 'TwitterHead' IoT Application
1. Configure & Connect to Twitter Node (authorize app & set node to listen for keywords, hashtages, or users)
2. Sentiment Node passes Msg to Switch Node which routes the Msg based on it's 'sentiment.score' value. 
3. Connect Switch Node to Trigger Nodes to send 1 (ON) or 0 (OFF) to Raspberry Pi GPIO Pinout Node(s).
4. Connect the Trigger Nodes to Raspberry Pi GPIO Pinout Nodes to fire the 'neurons' (LEDs) in the TwitterHead.
5. Send Msg.payload to Debug Node to diagnose any errors.   

#### Testing the Setup 

Below is a video of an early prototype in action. The Node-RED server is running on a Raspberry Pi running Raspbian (Stretch) on a 32GB micro-SD card. The debug node is configured to send the message stream to a console output, which I access through SSH on an iPad with a terminal emulator called [Terminus](https://www.termius.com). The Node-RED flow listens for tweets such as (#Westworld,#AI,#MachineLearning) and flashes red, white or multi-colour depending on the sentiment value of the tweet. Not only can the node be configured for #hashtags, it can also be used for @users and other tags as well. More information on the nodes used in this flow can be found [here](https://www.npmjs.com/package/sentiment) & [here] (https://www.npmjs.com/package/node-red-node-twitter)

[![Alt text](https://img.youtube.com/vi/HNA7sXDd9Sg/0.jpg)](https://www.youtube.com/watch?v=HNA7sXDd9Sg)

#### Future Directions 
The possibilities and directions for improvements are considerable, from improving the sentiment and language analyzer function by running tweets through Google Cloud or Amazon Web Services API's (Google Cloud Natural Language, AWS Comprehend),  plugging in new APIs, to connecting to other sensors and source of data such as the Muse EEG headset and improving the flow and codebase of the application.  





