In this project, to aid in the ongoing development and experimentation of use of AR in education, an AR based app will be developed. The app will be able to in-tegrate 3D models used in engineering education, mainly electronics and mechan-ical and allow students to view them in the context of real environment. The pro-ject will contribute in the field of educational AR apps by developing a new app as a supplemental tool for improving teaching. The current scope of the project will develop a prototype with limited opensource 3D models, interaction abilities, teaching content and quiz feature. 
5	PROJECT OVERVIEW
This project will develop an Augmented Reality mobile application to improve quality of teaching in engineering education. (While this project focus on using 3D models for engineering topics, the models can be for any education topic.) The app will display the models required to be taught in engineering courses in 3D interface. The students will be able to interact with the model using touch inter-face to rotate, translate and scale. For each model, a help menu will be provided on how to interact with it. Each model will also have a hotspot point on it where students can touch to find more information about that component. In addition, there will be a quiz mode where questions about the model will be asked to ac-cess student knowledge. 
5.1	Main features 
The main features of the project can be listed as follows:
1.	Develop an augmented reality mobile app based on Android OS
2.	Integrate various 3D models used in engineering education in the app
3.	Implement object detection to combine virtual model with real environ-ment (E.g. Engine in a car)
4.	Allow students to engage with the model with interactions such as rota-tion, scaling, translating etc. using touch and device orientation input
5.	Provide help, tutorial, demo modes to help students use the tool
6.	Provide hotspots on the model to get more information about the part of the model and overall information about the model
7.	Provide at least two types quiz based on the models to access student learning
a.	Multiple choice quiz on the overall model displayed
b.	Multiple choice quiz to identify part/points of the model
c.	Track the scores and provide feedback to students
8.	Integrate 3D models with more than one component
a.	Allow students to interact each component separately
b.	Also have a mode to see how different components combine to-gether to form a larger model
c.	Allow students to view and interact with the components com-bined
# Cryptogame User Manual

Cryptogame is android application cryptogram puzzle game that uses simple substitution cipher to encrypt the letters of a short sentence. The player has to decode the encrypted sentence and reveal the original one. Though it sounds easy just to replace the letters, it is a challenging but fun game. You can solve it out guessing the frequency of letters and their patterns in words. (*Hint*: Start with one letter word and look for most repititive letters - they belong to the *ETAOIN* group.) 
So try them out and good luck with the game!!

## System Requirements

- **Minimum SDK Required**: Android 6.0 or higher 

- **CPU**: 1.2 GHz or higher

- **RAM**: 1.0 GB or higher

- **Desktop usage**: Android Studio 3.3 or later versions required.

## Installation 

### Installing the app from source

1. Clone or Download the repository from following URL:

```https://github.gatech.edu/gt-omscs-se-2019spring/6300Spring19Team14/tree/master/GroupProject/```

2. Import Project Cryptogame in Android Studio.
3. To run you either need to connect your android phone with usb to the computer with developer option enabled or select one of the android emulators in Android Studio
4. Select ***Run app*** from **Run Menu** in Android Studio.
	- To run in your mobile select your phone in the list
	- To run in android studio emulators 
		1. Press ***Create New Virtual Device***
		1. Select one of the phones and then one of the releases and click finish
5. The app is ready for use.

**Install using APK**

1. Copy `Cryptogame.apk` from the `/APK` directory to an Andorid phone.
2. Open the copied `.apk` file in the phone and allow it be installed.
	
## Using the app

- The app has two user types: **Admin** and **Player**. 
- The administrator is able to create new players, crytogram games and view all the player statistics. 
- The players can choose and solve the cryptograms and view the player statistics.

### Features for the Admin

#### Login
1. Start the application.
2. Enter your username.
3. Click on ***Login*** button.

### Add a new player
1. After logging in click on ***Create PLayer*** button.
2. In the form, enter *first name*, *last name* and *unique username* in the provided fields. The maximum number of characters allowed for each field is 30.
3. Select the difficulty level for the player.
4. To add the player, click on ***Add Player*** button and to clear all the fields press ***Reset*** button.

### Add a new cryptogram
1. After logging in, click on ***Create Cryptogram*** button.
2. In the form, enter *unique cryptogram name*, the sentence for which encrypted phrase is generated. The *encrypted phrase* is self generated. The maximum number of characters allowed for cryptogram name is 30 and the cryptogram solution needs to have at least one alphabet.
3. Enter *the number of incorrect solutions* allowed for solving the cryptogram for *easy* , *normal* and *hard* difficulty levels in the provided fields. The values for each level has to be greater than 0(This is checked by the application).(But, the admin has to make sure the order of the values he enters for each level, whether they are meaningful. The application leaves that choice to the admin!)
4. Edit any of the fields before saving.
5. To add the cryptogram, click on ***Save*** button and to clear all the fields press ***Reset*** button.

### View Player Statistics
1. After logging in, click on ***View Player Statistics*** button.
2. The list of players with their *first name*, *username*, *difficulty level*, *number of wins* and *number of losses* generated can be viewed.

### Logout
1. After logging in, logout of the app at any time using the ***Logout*** button at the Admin Menu.


### Features for the Player

#### Login
1. Start the application.
2. Enter your username.
3. Click on ***Login*** button.

#### Choose and then solve cryptogram
1. After logging in, click on ***Choose Cryptogram*** button.
2. Select either **not started** or **in-progress** cryptogram from the list displayed. The *encrypted phrase* is self generated when the player clicks a new **not started** cryptogram.
3. The *cryptoname* and *number of allowed incorrect attempts* for player's difiiculty level is available at the top.
4. The encrypted phrase can be seen below the remaining attempts and for every unique letter, a blank space is provided to input assumed probable letter. 
4. Enter probable letters in the blanks tallying with the encrypted phrase letters.
5. Clear all the fields or the errors using ***Reset*** button at any time. 
6. Return back to menu at any time. The app saves the state of the game by saving your potential solution and marks it as **in-progress**. The game can be resumed later from the list of crytograms.
7. After filling in all the blanks, view the *potential solution* that has been entered before submitting the answer by ***View Potential Solution*** button. (Every time you modify letters, make sure to save your solution before exiting the game to preserve the state!)
8. Once all the blanks are filled and satisfied with the potential answer, submit with ***Submit Answer*** button. The player must click on ***View Potential Solution*** button to enable ***Submit Answer*** button.
9. The player is informed by a message either if the solution submitted was correct or incorrect. 
 	- If solution is correct, the game is won then the cryptogram is marked as completed. 
	- If the solution is incorrect, the number of attempts is decreased but still appears in cryptogram list as **in-progress** but with blank fields when the game is started. The unsolved game is also marked as completed and lost game if the number of attempts is equal to zero. 
	- In either completed case, the game is removed from the ***Choose Cryptogram*** to-solve list. 

### View Player Statistics
1. After logging in, click on ***View Player Statistics*** button.
2. The list of players with only their *first name*, *number of wins* and *number of losses* generated can be viewed. This list will display in descending order of number of cryptograms won.


### Logout
1. After logging in, logout of the app at any time using the  ***Logout*** button at the Player Menu.	


