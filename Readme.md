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



### Training the model
-> Add the layers
-> get the weights and bias of your neural network

### Test the model

### Get the score
