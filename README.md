# Optimal-Chess-Moves
The goal of this project is to allow a player to take a picture of the chess board and have an algorithm tell you the optimal move.


# Note:

I can't affor a decsent computer that has GPU, this is why any object detection model training will be done using Google Colab. I paid for the $9.99 pro version so that I could use their faster cloud GPU without worrying about the kernels restarting every 30 minutes. 

# Dataset:

I created a custom dataset of labeled chess peices. I used a program called Labelme to draw bounding boxes around all chess peices on the board. 

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




