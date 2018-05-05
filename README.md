# Doanything
just throw your ideas here and there!
del mydata.column_name
mydata.drop('column_name', axis=1, inplace=True)

from sklearn.preprocessing import Imputer
values = mydata.values
imputer = Imputer(missing_values=’NaN’, strategy=’mean’)
transformed_values = imputer.fit_transform(values)

In python
from fancyimpute import KNN    

# Use 5 nearest rows which have a feature to fill in each row's missing features
knnOutput = KNN(k=5).complete(mydata)
