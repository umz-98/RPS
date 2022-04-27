# Computer vision project

## Milestone 1 - 'Talk about the model and how you will use it for this project.'

To start of the project an image project model was made using a teachable machine. This model has stored many images that result to the following elements: rock, paper, scissors and nothing. Essentially this is the core of this project that makes the game work. Now that the model is complete the model was run on the computer using a code. The aim was to see if the model works properly by checking if the camera rightfully identifies the elements using hand signs. The information would be written into a code that would act as the user’s choice in the game.


## Milestone 3 - 'Talk about how you setup your environment and the code you have written for the game'

### The environment 
The environment was created using conda commands by first downloading miniconda. Miniconda is a minimal installer of conda which was needed for the next steps. The environment was than created by using ‘conda create --…’ whereby the environment was named as ‘test’. Following the creation of the environment it was activated using ‘conda activate test’. Following the completion of setting up the environment, ‘pip’ was used to allow OpenCV and TensorFlow to be installed (Pip install….). These libraries would be present in this environment therefore the previously downloaded model was moved into the directory where this environment was found.

### The code
A random.choice()= code was used for the computer with the options being ‘rock’, ‘paper’, ‘scissors’ and ‘nothing’ to generate the choice it makes. On the other hand, if-else statements inside a function were used to generate the users choice with the same options. Following this If-else statements were used inside another function to write a code that would explain the conditions and declare a winner of the rock, paper and scissors game. Whilst at this point the code for this was different to what it changed to at the end most of it remained the same. The change that was made was adding Booleans for the score which changed the function. Another change was that the computers code to select an option was also added into this function.

#### Webcam
Whilst the ‘messages’ that will be displayed onto the screen were being written it was apparent that they don’t fit the webcam size. Therefore, in the code: 
'cv2.putText(frame,message, (30,30), cv2.FONT_HERSHEY_DUPLEX, 0.75, (0, 0, 255), 1)'
The font size (0.75) was reduced so the message is clearly visible in the webcam.

## Final Milestone 

The game is completed and it functions using the traditional rules of a rock, paper and scissors game, but it also has some extra features which will be described below. 

A countdown has been added to allow the user to have time to put their choice of rock, paper or scissors up. There is also an option of ‘nothing’ for both the computer and the user this therefore gives both side equal probability of picking any of the options. Whilst it is true ‘nothing’ is not an option it is crucial as it allows the computer to understand ‘nothing’ has been shown if the user was too late to pick a choice. The game has been formatted in such a way that neither the computer nor the user benefit from the ‘nothing’ option. This game also incorporates a score which gives one point if the right conditions are met for both the computer and the user. The reason the computer has been given a score is solely to allow for a competition where the user can lose too rather than just the user trying to win. The game provides a message following the win of three rounds for both, hence allowing there to be a final to the game rather than an endless game. However, at the same time it is possible to carry on if the user wishes so. 

Overall the only downside to this game is losing to the computer…

### To improve
Whilst I believe the conditions for a traditional rock, paper and scissors game have been met there are always ways to improve. Therefore, one way to improve this game would be training the initial model even more. This could be done through various ways including: choosing different angles of the camera, different clothes, more angles of the shapes or even including other people. This would be a great improvement as one should understand that the game doesn’t necessarily have to be played in the same conditions as how the model was developed. Things like lightening and angles can make a huge difference. Involving other people has also been mentioned so that other people can play this game the same way. Different hand shapes, fingers and nail sizes can make a great difference too. All in all, incorporating all these things can drastically help improve the model and the quality of the game.

A more advanced way of improving the game would be including levels and a ‘highest score’. As the rock, paper and scissors game does not change the levels would not be regarding difficulty but just by how many levels (one level would equate to winning 3 rounds) one can win. The highest score a more simple and straightforward improvement could also be added. This value could just result in the longest run you have had regardless of how many times the computer won too. Another way it could be added is the number of times you won in e.g. two minutes. This would allow people to compete with each other to increase the number of times one can win in playing the game for 2 minutes straight.
