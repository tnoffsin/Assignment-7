# Assignment-7
#The thing I was asked to accomplish
Write a function that makes individual lists for each unique loan_intent value and include in these lists the most common loan_grade, average loan_amnt, and average loan_int_rate and write it to a new CSV file.
#This is the columns and types of data recorded in my dataset
Loan dataset columns: customer_id: Unique identifier for each customer customer_age: Age of the customer customer_income: Annual income of the customer home_ownership: Home ownership status (e.g., RENT, OWN, MORTGAGE) employment_duration: Duration of employment in months loan_intent: Purpose of the loan (e.g., PERSONAL, EDUCATION, MEDICAL, VENTURE) loan_grade: Grade assigned to the loan loan_amnt: Loan amount requested loan_int_rate: Interest rate of the loan term_years: Loan term in years historical_default: Indicates if the customer has a history of default (Y/N) cred_hist_length: Length of the customer's credit history in years Current_loan_status: Current status of the loan (DEFAULT, NO DEFAULT)

#Summary of how the code works.
First it starts by importing and reading the CSV file. Then uses safe_float funciton to convert a value to a float. If there is a error then it returns None. Then it reads the loan data from the input CSV file and processes it, and whites and output CSV file. csv.DictReader reads the CSV file into a list of dictionaries where each dictionary represents a row with column names as keys. It then groups the individual rows by loan_intent column. Then collects all the columns and Find the most common loan grade using count. Afterwards it calculates the average loan interest rate. It then appens the calculated statistics for each loan intent to the results_data list. It then writes the resultant data into a new CSV file.

#examples of Lists in the code if any
csv.DictReader reads the CSB file and returns each row as an ordered dictionary. This is converted  into a list of dictionaries named data.

defaultdict is a list used to group rows by the balue of the loan_intent column. The grouped_data dictionary has keys corresponding to different loan intents and the values are lists of rows that share the same loan intent. 

Another example would be 
loan_grade, loan_amnt, loan_int_rates and all lists  and collects data from the dataset and stores them into seperates labeled with the same label such as, loan_grade, loan_amnt, loan_int_rates. 

#Why is this important
It is important because it helps with summarizing and analyzing large datasets, you can also make meaningful patterns and trends that make with informed decisions. It also helps with dealing with large amounts of data, and helps automating processes which can be extremely helpful. 


