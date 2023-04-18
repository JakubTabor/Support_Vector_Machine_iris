# Support_Vector_Machine_iris
# First i save my "iris" data """iris = load_iris()""" and load it into columns """df = pd.DataFrame(iris.data, columns=iris.feature_names)""" save it as a "df"
# Then I create new column "target" """df['target'] = iris.target""" 
# And set "flower_name" on my column "target" """df['flower_name'] = df.target.apply(lambda x : iris.target_names[x])"""
