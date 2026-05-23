# From Dataset Analyzing to model creating

### <ins> Analyzing Dataset </ins>

-> **df.info()** : figure out the Data Type, Null values   
-> **df.duplicate().sum** : duplicates rows <br>
-> **df[' '].value_counts()** : for listing unique values of a paricluar columns <br>
-> **df.drop(columns = ['  ' , '  '])** : Remove non required columns <br>
-> **df.get_dummies(df, columns=[' ',' '], drop_first = True)** : get 0/1 of your character columns <br>

### <ins>Plot scatter graph between two columns</ins>

° Like Price and area 

sns.scatterplot(data=df, x="RM", y="PRICE");

### Split your values (train_test_split)



### Scale your values



### <ins>Training Configuration</ins>

-> initialize model (model = Sequential)  
-> Add the layers or hidden layers(model.add(Dense(No. of nodes), activation='sigmoid/relu'), input_Dim=11)    
-> get the weights and bias of your neural network

° If it is in 2D array, we need to flatten the data before initilizing hidden layer  
model.add(Flatten(input_shape=(28,28)))

<ins>Get summary of your layers</ins>
model.summary()
-> Summary  
-> No. of Parameters (weights+ bias)  

##### Mention the loss and optimizer
loss: If result is either 0/1 or class use binary_crossentropy or log loss and if it is any multiple class prediction use sparse_categorical_crossentropy or categorical_crossentropy  
Optimizer : Adam

sparse_categorical_crossentropy or categorical_crossentropy - in sparse you don't need to do one hot encoding like identifying digits(1 to 9) and in categorical you need to do first one hot encoding  

syntax: 
model.compile(loss='binary_crossentropy', optimizer='Adam')  


### Training the model  
model.fit(X_train_scaled, y_train, epochs=50)

### Test the model  

### Get the score  
  
  
## Notes  
° When you have output layer more than 1, use softmax activation function  
° For hidden layer preffered relu then sigmoid  
