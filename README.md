# knn_exercise_digits_solution
# First I save digits """digits = load_digits()""", then I look at description of my data 
# I create my "df" using "digits.data" and "digits.target" """df = pd.DataFrame(digits.data, digits.target)"""
# Then I create new column "target" """df['target'] = digits.target"""
# I have my "df" prepared so I can import "train_test_split" and get "train" and "test" set 
# "X" will be my "df" without column "target" and "y" my "df.target"
