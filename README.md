# Support_Vector_Machine_iris
# First i save my "iris" data """iris = load_iris()""" and load it into columns """df = pd.DataFrame(iris.data, columns=iris.feature_names)""" save it as a "df"
# Then I create new column "target" """df['target'] = iris.target""" 
# And set "flower_name" on my column "target" """df['flower_name'] = df.target.apply(lambda x : iris.target_names[x])"""
# I save (3) df to each of my "flower_name" "df0 = df[df.target==0]" "df1 = df[df.target==1]" "df2 = df[df.target==2]"
# Then plot my data on "scatter.plot" and set parameters "Sepal length" and "Sepal width" from my "df0" and "df1"
# And exactly I do this same with "petal length" and "petal width"
# I import my "train_test_split" and set my "X" as my df, without column "target" and "flower_name" """X = df.drop(['target', 'flower_name'], axis='columns')"""
# And "y" is my "targert" column """y = df.target""", then i get my "train" and "test" set
# Next i get "SVC" model and train my data """model.fit(X_train, y_train)"""
# And get "score" """model.score(X_test, y_test)"""
