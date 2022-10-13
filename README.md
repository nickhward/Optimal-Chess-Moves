# Optimal-Chess-Moves
The goal of this project is to allow a player to take a picture of the chess board and have an algorithm tell you the optimal move.


# Note:

I can't affor a decsent computer that has GPU, this is why any object detection model training will be done using Google Colab. I paid for the $9.99 pro version so that I could use their faster cloud GPU without worrying about the kernels restarting every 30 minutes. 

# Dataset:

I created a custom dataset of labeled chess peices. I used a program called Labelme to draw bounding boxes around all chess peices on the board. 

Training set   : 400

Validation set : 100

Testing set    : 100

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


