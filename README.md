# Shoe-type-detector
This project shows the detection of 3 different shoe types. In our daily life, there are different types of shoes for us to choose. However, different shoes are needed for different occasions. This AI can help you detect the type of shoe is in the picture. The shoes would be detected into 3 types: sneakers, loafers, and slippers. 

# The Algorithm
This program utilizes imagenet through the help of Nvidia's Jetson Nano Kit. It uses imagenet to sperate different shoes into classIDs and then provide the results.  

# Running the Program
1. Connect to the Jetson Nano Kit throught the ip address recorded
2. Open Visual Studio code and connect to Nano using the IP address found in the previous step
3. Choose pictures that you would like for this AI model to detect and (if needed) change the pictures into JPG files
4. Put the pictures that you chose into the same directory as to where the python file is - "imagenet.py"
5. Write the following command in the terminal - python3 imagenet.py [name of ur pic].jpg [name of the pic after detected].jpg
