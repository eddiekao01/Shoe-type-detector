# Shoe-type-detector
This project shows the detection of 10 different kitchen utensils. It helps people identify the most common different utensils and cooking ware. There are 10 different kitchenm utensils used: a cheese grater, ladle, large spoon, meat tenderizer, pie server, slotted spoon, spaghetti server, spatula, tongs, and a whisk. This AI was created because I struggled with differentiating the names of a couple of kitchen utensils, this AI helps me do that.

This project shows the detection of 3 different shoe types. In our daily life, there are lots of different types of shoes for us to choose. However, there are different shoes needed for different occasions. This AI can help you detect the type of shoe is in the picture. The shoes would be detected into 3 types: sneakers, loafers, and slippers. 
The Algorithm
My program utilizes imagenet and resnet-18. It uses imagenet to views the live video feed and train the images. Resnet-18 is the base of the AI program. After taking all the pictures and training the dataset, start the live video feed and classifying the images. It uses torch and torchvision to train the model, resnet-18 as the base for my network, and the live video feed to run the imagenet program to classify the utensils.

Running the Program
Login into your nano
Click on code and download as a .zip file, upload and unzip in nano under the jetson-inference/python/training/classification directory
cd back to jetson-inference
Run the docker using docker/run.sh
cd into python/training/classification
Train the data by using: python3 train.py --model-dir=models/kitchen --batch-size=4 --workers=1 data/kitchen
To run the code, type: imagenet --model=models/kitchen/resnet18.onnx --labels=data/kitchen/labels.txt --input-blob=input_0 --output-blob=output_0 /dev/video0
Show one of the 10 following items:
cheese grater
ladle
large spoon
meat tenderizer
pie server
slotted spoon
spaghetti server
spatula
tongs
whisk
Required Libraries Needed

resnet-18
imagenet
View a Video Demonstration Here https://youtu.be/bf507Dtj4Wk
