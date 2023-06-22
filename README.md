# Module11Challenge

https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.astype.html
When using the astype method in part 2 step 4.

AskBCS assistant helped me with the following code in part 2.
# Create an empty list
data = []

# Loop through the scraped data to create a list of rows
# Iterate over the rows and extract the data
for row in rows:
    td = row.find_all('td')
    row = [col.text for col in td]
    data.append(row)

# Create a Pandas DataFrame by using the list of rows and a list of the column names
df = pd.DataFrame(data, columns = ['id', 'terrestrial_data', 'sol', 'ls', 'month', 'min_temp', 'pressure'])
