# knn_exercise_digits_solution
# First I save digits """digits = load_digits()""", then I look at description of my data 
# I create my "df" using "digits.data" and "digits.target" """df = pd.DataFrame(digits.data, digits.target)"""
# Then I create new column "target" """df['target'] = digits.target"""
# I have my "df" prepared so I can import "train_test_split" and get "train" and "test" set 
# "X" will be my "df" without column "target" and "y" my "df.target"
# Now I can import "KNeighborsClassifier" and I set parameter "n_neighbors" at (5) """knn = KNeighborsClassifier(n_neighbors=5)"""
# I check length of my "X_train" nad "X_test", "len(X_train)" "len(X_test)", then i train my classifier """knn.fit(X_train, y_train)"""
# And get "score" """knn.score(X_test, y_test)""" and prepare my using classifier "y_pred" """y_pred = knn.predict(X_test)"""
# I import "confusion_matrix" and put into my "y_test" and "y_pred" """cm = confusion_matrix(y_test, y_pred)"""
# Ten i use "%matplotlib inline" and "seaborn" to visualize my results and I use "confusion_matrix" """sn.heatmap(cm, annot=True)"""
