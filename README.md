# CME-Data-Scraper
The CME Group Futures Data Scraper is a Python script that enables users to retrieve futures data from the CME Group API and transform it into a structured format for analysis. The script offers a convenient way to access and process financial data from the Chicago Mercantile Exchange (CME) for a specified date.

## Prerequisites

Before running the script, make sure you have the following dependencies installed:

- Python (3.x)
- requests library
- pandas library

You can install the required Python packages using pip:

```
pip install requests pandas
```

# Explanation

1. Import necessary libraries:

```
import requests
import pandas as pd

```

2. Set the date variable to the desired date for fetching futures data from CME Group.
3. Construct the URL for the CME Group API endpoint, including the date parameter.
4. Define the headers required for making the HTTP request. Be sure to include any necessary cookies or authentication tokens in the 'Cookie' field (as it is omitted for brevity).
5. Use the requests.get() method to download futures data from the CME Group API.
6. Convert the JSON response from the API into a Pandas DataFrame, making it easier to work with and analyze.
7. Extract the 'settlements' data from the DataFrame using pd.json_normalize().
8. Concatenate the 'settlements' DataFrame with the original futures data DataFrame, creating a combined DataFrame.
9. Select and display the desired columns from the combined DataFrame, including 'month,' 'open,' 'high,' 'low,' 'last,' 'change,' 'settle,' 'volume,' 'openInterest,' 'tradeDate,' 'dsHeader,' and 'reportType'.

# Output

![alt text](https://raw.githubusercontent.com/sumitdnath/CME-Data-Scraper/main/image.png)

Capture and display screenshots of the script in action.





