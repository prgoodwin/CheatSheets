# Loading in a CSV
dataset = pd.read_csv('file.csv') 

# dataframe slicing using iloc
features = dataset.iloc[:,0:n]

## Last column
labels = dataset.iloc[:,-1]
## Everything but the last column
features = dataset.iloc[:,0:-1]
# Selecting the last column with -1 
labels = dataset.iloc[:,-1] 

# Shape
labels.shape[0]

# Describe
labels.describe())

# Turn String data into individual columns
pd.get_dummies(features)