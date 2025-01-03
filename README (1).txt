Instruction to execute the model on the test set from "execution.ipynb" file.

we saved the trained model in "cnn_model.pt" so we loaded it in the ipynb file 

1. Run the import statements in the first cell of the notebook.
2. Run the second cell to mount your drive into the environment.
3. Change the path to the saved model file accordingly in the immediate cell where it is mentioned.
4. Change the path to the test dataset in the next line accordingly.
5. Run all the cells from the current cell to the end of the file. (These cells load the image and resize them properly to fit the input size of the model)
6. These cells will load the test data predict them on the loaded model and print a classification report with accuracy and other scores.
7. Along with that we will get the confusion matrix to the predictions on the test data.
