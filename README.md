# SGD_classifier_OpenCV
This code generates FEN code according to the location of chess pieces, using the SGDClassifier machine learning model.

### chess peice detection

Original file is located at [colab](https://colab.research.google.com/drive/1M5BB_EwgD1bNF2B0JyGZMoe7sk59M2F3)


* This code generates FEN code according to the location of chess pieces, using the SGDClassifier machine learning model. 
* The method is similar to the famous MNIST problem. 
* The training data contains 18,000 chessboards.
*  The code then creates 60,000 images from these chessboards, each containing 64 squares, with up to 32 pieces in the game.
* example: FEN code: rnbqkbnr/pppppppp/8/8/8/8/PPPPPPPP/RNBQKBNR


## Libraries Used
* cv2
* numpy
* pandas
* glob
* os
* re
* tqdm
* matplotlib


## Functions
normalizeBoardName(boardName):

this function normalizes the FEN code.

## Process
* Introduction of the folder that contains the images.
* Define a function to normalize the FEN code.
* Creation of 60,000 images from the chessboards, where each board contains 64 squares and at most 32 pieces.
* Save the 60,000 images in an Excel file.
* Read the data from the directory.

## Exploratory Data Analysis (EDA) and Data Cleaning.
* Convert categorical features to numerical.
* Split the data into training and testing sets.

## train a model and prediction
* after trainig a SGDClassifier model we can simply predict the fen codes of each chess board


## Credits
Original file is located at [colab](https://colab.research.google.com/drive/1M5BB_EwgD1bNF2B0JyGZMoe7sk59M2F3)


* more info about fen: [fen_wiki](https://en.wikipedia.org/wiki/Forsyth%E2%80%93Edwards_Notation)

* the training data contains 18k chess board ( [G_drive](https://drive.google.com/file/d/1LQw3tHxbDzXJuZjcwJrwcJHzsYsp9ZfH/view?usp=share_link))
* the data for trainig the mode(60k-peice)( [G_drive](https://drive.google.com/file/d/1Elel68b2BhUqOxyytonA8iJeA-VL84sJ/view?usp=sharing) )
* the test data (the answers should be checked visually)( [G_Drive](https://drive.google.com/file/d/1Af65xO6ygKiX4TYeUpXbacGjDEvI6OZJ/view?usp=share_link))

Mnist data can load from google drive: [MNIST](https://drive.google.com/drive/folders/1IUyKdQw0YaK3R3ncbtSCYGak_7c6UiFG?usp=share_link)

