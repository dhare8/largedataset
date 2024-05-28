base_data=[
    {
        "Input": "Write a python code to drop column gender in a dataframe.",
        "Output": "df.drop(['gender'], axis=1, inplace=True)"
    },
    
    
    {
        "Input": "Write a python code to filter the data of column marks",
        "Output": "df[df['marks']>10]"
    },
    {
        "Input": "Write a python code to filter the data of column marks using query",
        "Output": "df.query('marks'>10)"
    },
    
    
    {
        "Input": "Write a python code for grouping and aggregating the data.",
        "Output": "df.groupby('gender').sum()"
    },
  
    {
        "Input": "Write a python code to find mean of column marks.",
        "Output": "df['marks'].mean()"
    },
    {
        "Input": "Write a python code to find median of column marks.",
        "Output": "df['marks'].median()"
    },
    {
        "Input": "Write a python code to find mode of column marks.",
        "Output": "df['marks'].mode()"
    },
    {
        "Input": "Write a python code to find standard deviation of column marks.",
        "Output": "df['marks'].std()"
    },
    {
        "Input": "Write a python code to find variance of column marks.",
        "Output": "df['marks'].var()"
    },
    {
        "Input": "Write a python code to find correlation of column marks with result.",
        "Output": "df['marks'].corr(df['result'])"
    },
    {
        "Input": "Write a python code to find covariance of column marks with result.",
        "Output": "df['marks'].cov(df['result'])"
    },
    
    {
        "Input": "Write a python code to create a new column 'status' based on the condition that marks greater than 50 is 'Pass' else 'Fail'.",
        "Output": "df['status'] = df['marks'].apply(lambda x: 'Pass' if x > 50 else 'Fail')"
    },
    {
        "Input": "Write a python code to calculate the maximum value of the 'height' column.",
        "Output": "df['height'].max()"
    },
    {
        "Input": "Write a python code to calculate the minimum value of the 'height' column.",
        "Output": "df['height'].min()"
    },

    {
        "Input": "Write a python code to select rows where the 'country' column is equal to 'USA'.",
        "Output": "df_usa = df[df['country'] == 'USA']"
    },
    {
        "Input": "Write a python code to apply a lambda function to square each element in the 'score' column.",
        "Output": "df['score'] = df['score'].apply(lambda x: x**2)"
    },
    
    {
        "Input": "Write a python code to get unique values in the 'city' column.",
        "Output": "df['city'].unique()"
    },
    {
        "Input": "Write a python code to count unique values in the 'city' column.",
        "Output": "df['city'].nunique()"
    },
    
    {
        "Input": "Write a python code to normalize the 'sales' column.",
        "Output": "df['sales_normalized'] = (df['sales'] - df['sales'].min()) / (df['sales'].max() - df['sales'].min())"
    },
    {
        "Input": "Write a python code to replace values greater than 100 in column score with 100.",
        "Output": "df['score'] = df['score'].apply(lambda x: 100 if x > 100 else x)"
    },
    {
        "Input": "Write a python code to create a cumulative sum column for 'sales'.",
        "Output": "df['sales_cumsum'] = df['sales'].cumsum()"
    },






        
        {
            "Input": "Write a python code to create a pivot table with 'sales' as values and 'month' as index.",
            "Output": "pd.pivot_table(df, values='sales', index='month')"
        },
        
        
        {
            "Input": "Write a python code to create dummy variables for a column 'category'.",
            "Output": "pd.get_dummies(df['category'])"
        },
        {
            "Input": "Write a python code to factorize the 'category' column.",
            "Output": "df['category'] = pd.factorize(df['category'])[0]"
        },
        
        {
            "Input": "Write a python code to convert a column 'price' to numeric.",
            "Output": "df['price'] = pd.to_numeric(df['price'])"
        },
       
       
        {
            "Input": "Write a python code to filter rows where 'city' is in a list of cities.",
            "Output": "df[df['city'].isin(['New York', 'Los Angeles'])]"
        },
        
        {
            "Input": "Write a python code to add two columns 'price' and 'tax' and store the result in 'total'.",
            "Output": "df['total'] = df['price'] + df['tax']"
        },
       
        {
            "Input": "Write a python code to apply a function to a column 'price'.",
            "Output": "df['price'] = df['price'].apply(lambda x: x * 1.1)"
        },
        {
            "Input": "Write a python code to map values in 'category' column using a dictionary.",
            "Output": "df['category'] = df['category'].map({'A': 1, 'B': 2})"
        },
       
        {
            "Input": "Write a python code to transform the 'sales' column by subtracting the mean.",
            "Output": "df['sales'] = df['sales'].transform(lambda x: x - x.mean())"
        },
    
       
        {
            "Input": "Write a python code to sort the dataframe by 'price'.",
            "Output": "df.sort_values(by='price', inplace=True)"
        },
        {
            "Input": "Write a python code to replace values in 'category' column.",
            "Output": "df['category'].replace({'A': 'Alpha', 'B': 'Beta'}, inplace=True)"
        },
        
        {
            "Input": "Write a python code to filter the dataframe for rows where 'age' is not null.",
            "Output": "df = df[df['age'].notnull()]"
        }  
]
