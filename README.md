# Support_Vector_Machine_iris
# First i save my "iris" data """iris = load_iris()""" and load it into columns """df = pd.DataFrame(iris.data, columns=iris.feature_names)""" save it as a "df"
# Then I create new column "target" """df['target'] = iris.target""" 
# And set "flower_name" on my column "target" """df['flower_name'] = df.target.apply(lambda x : iris.target_names[x])"""
# I save 3 df to each of my "flower_name" "df0 = df[df.target==0]" "df1 = df[df.target==1]" "df2 = df[df.target==2]"
