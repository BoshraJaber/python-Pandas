# Lab: 12 - Data Analysis with Pandas

```  poetry config virtualenvs.create true ```

## Implementation Notes
* poetry add jupyterlab
* poetry add pandas
* poetry shell

## Notes:
* **Kaggle**: we use it to get data
* import pandas as pd
* df = pd.read_csv('./cereal.csv') // to read the file
* df.info() // to check info about the file
* df.head() // to show top rows
* df.tail(10) // to show last 10 rows
* df[["name", "mfr"]] //  filter the df by columns name and mfr
* df.set_index("fat") # set which colum to be your index (the first column)
* new_df = df[["name","rating","sugars"]].sort_values('rating', ascending=False) // sprting
* avg_sodium = df[["sodium"]].mean() // fining average
* max_carbohydrate = df['carbo'].max() // finding max
* highly_rated_food =  df[df['rating'] > 50][['name', 'sugars']] // Show the food name and sugar content of any food with a rating larger than 50
* mcc =  df['carbo'].mode() // 
* df['potass'].std() // standard deviation
* enumerate() allows us to iterate through a sequence but it keeps track of both the index and the element. The enumerate() function takes in an iterable as an argument, such as a list, string, tuple, or dictionary.