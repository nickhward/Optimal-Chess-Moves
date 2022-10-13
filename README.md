# Optimal-Chess-Moves
The goal of this project is to allow a player to take a picture of the chess board and have an algorithm tell you the optimal move.


# Note:

I can't affor a decsent computer that has GPU, this is why any object detection model training will be done using Google Colab. I paid for the $9.99 pro version so that I could use their faster cloud GPU without worrying about the kernels restarting every 30 minutes. 

# Dataset:

I created a custom dataset of labeled chess peices. I used a program called Labelme to draw bounding boxes around all chess peices on the board. 

![Screen Shot 2022-10-08 at 1 03 03 PM](https://user-images.githubusercontent.com/78880630/195529572-3f3a29f1-54b9-44f7-befe-174ef68b9a10.png)

Upload your custom dataset into roboflow, it will split your data into a train, validation, test split of your choosing. Another cool feature is that you can export the data in the format you need for the model you plan on using. It is free for private/research use. 



Training set   : 1300

Validation set : 127

Testing set    : 63

Naming Convention of Pieces: 

| Peice Name     | Label |
| ---      | ---       |
| White Bishop | WB         |
| White King     | WK        |
| White Pawn | WP         |
| White Knight     | WKN       |
| White Qween | WQ         |
| White Castle     | WC        |
| Black Bishop | BB         |
| Black King     | BK       |
| Black Pawn  | BP         |
| Black Knight     | BKN        |
| Black Qween     | BQ        |
| Black Castle     | BC|        |

Augmentation of Images:

This is useful to add more training examples for the model to learn

- Flipped
- Rotation of 90 Deg
- Shear
- Grayscale
- Brightness

Example of final image with labeling:

![Screen Shot 2022-10-13 at 12 27 47 AM](https://user-images.githubusercontent.com/78880630/195530437-18bf3214-342d-4dd9-8831-5d4d0d58e31b.png)


# Results:

![image](https://user-images.githubusercontent.com/78880630/195548452-5aa7ab9c-4499-4544-b4c3-d1dc2b71f71a.png)

![image](https://user-images.githubusercontent.com/78880630/195548480-b1e89115-42cc-4c8b-b7b0-1645d39e3fd5.png)

![image](https://user-images.githubusercontent.com/78880630/195548536-5989443e-c95d-48d3-9b7e-94285f50f2f5.png)

![image](https://user-images.githubusercontent.com/78880630/195548596-21ae18db-6b2a-489f-a7f7-2539a0036cef.png)

![image](https://user-images.githubusercontent.com/78880630/195548654-2f95b01e-3e57-427f-a599-fbf14ffa070a.png)






