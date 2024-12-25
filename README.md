# Volleyball Ball Highlighter
Volleyball clip tracker for player clips for highlighting clips and making ball movements easier to see. As a former volleyball player, I see clips or highlights of my friends and peers. However, sometimes its hard to keep track of players and balls, especially in non-professional videos. So, here's a ball tracker for volleyball clips. 

## Future Steps
Expand to a player tracker, to see track each individual players for personal highlights. This would be beneficial for clip compilations for atheltes who want a highlight reel to share.
Expand the dataset with more court angles, types of games (professional and recreational), and number of clips. 

# Making a Roboflow Dataset 
Split a short volleyball into its frames and manually annotated each image with classes (player, ball, referee). 
![image](https://github.com/user-attachments/assets/7cba5c5e-4a93-407f-9622-0acf74c4ffc4)
Although Roboflow 3.0 Object Detection had high precision measures, the dataset is too small.
Dataset can be found here: https://universe.roboflow.com/vb-mprtn/vb-0hnak

# Object Detection Results
Trained for best.pt, last.pt model weights using YOLOv8 after 100 epochs. Furthering the dataset will help increase consistency and accuracy. 

Here are the results.  

## For professional clips:
https://github.com/user-attachments/assets/56ceba29-eed9-4adc-8966-3fca857e1a1e

## For non-professional clips: 
https://github.com/user-attachments/assets/0c198af6-6be3-4b18-9e31-c4a7c62c05a5

Non-professional clips are clearly less accurate. Picking up sideline players, and crowd members. Hopefully expanding the dataset with more non-professional images will help and improve accuracy.

# Ball Highlighting Results 

https://github.com/user-attachments/assets/bcced134-1e53-4e32-ab54-3bd3d232e4da

Frame rate has been slightly slowed to see accuracy of tracking of the ball frame by frame. 

# Acknowledgements 
Thanks to Code In a Jiffy on Youtube for tracking shapes and help. :) https://youtu.be/neBZ6huolkg?si=78i6rApdLd6iAuT9
