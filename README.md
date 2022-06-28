# Final-Project

The Project is basically to make predictions by using different ML models By passing arguments that is the attriutes which is used to predict the value accorrding to the model . 
Like in the Iris_Flower_Prediction attributes which is required is    pattle length-pattlel width-sepal length-sepal width and so on .
All this is be done in a py file that contains main function and models is called like a function.

All this is done by the Save and Restore method in the python having Modules like PICKLE.

To save the model all we need to do is pass the model object into the dump() function of Pickle. This will serialize the object and convert it into a “byte stream” that we can save as a file called model.

Loading library
  ## import pickle

To save the model syntax will be 
  
  # create an iterator object with write permission - model.pkl
    with open('model_pkl', 'wb') as files:
      pickle.dump(model, files)
  
To load the model syntax will be

  # load saved model
    with open('model_pkl' , 'rb') as f:
      lr = pickle.lload(f)

Now when we make prediction we try 

  # predict
    lr.predict(X_test)     OR   lr.predict([[5000-perticular value]])




There is another way to do same , to save and restore model by using JOBLIB 

# what is the use of Pickle ?
     It is the method by which we can make model trained ie. we don't need to train our model every time when we change the system or the environment . 
     we simply just make the prediction of an integer value or range of the value.
     It is such a useful tool to the ease of the prediction.
