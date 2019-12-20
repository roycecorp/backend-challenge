# Coding Challenge - Backend Developer
Create a TypeScript Node.js application that fetches all the files in this repository and displays a list of files and folders in a tree-like format in the console. Use the GitHub REST API v3 to fetch the list of files and folders in this repository. For every folder you find, you will have to make additional calls to the GitHub API to get its contents, and keep crawling through the results until you're done fetching all the folders in the repository.

The output of the program should be similar to the following example:

```
+ ABC
  + Atlanta
    - AAPL_data.csv
    - ABBV_data.csv
    - ABC_data.csv
  + Boston
    - ABT_data.csv
    - ACN_data.csv
    - ADBE_data.csv
  + Chicago
    - ADI_data.csv
    - ADM_data.csv
    - ADP_data.csv
  - A_data.csv
  - AAL_data.csv
  - AAP_data.csv
+ DEF
  + Denver
    - ADS_data.csv
    - ADSK_data.csv
...
- AVY_data.csv
- AWK_data.csv
- AXP_data.csv
- README.md
```



## Game rules and hints
- Google is your friend. You can use Internet resources to help you solve this challenge
- You should be able to understand and explain all the code you deliver
- The source code has to be valid TypeScript code. While it's possible to use `ts-node` to run your code, we would much rather see you transpile/convert the source code into JavaScript files and have use `node` to run them
- You can use the features available in ES2017
- It's highly desirable (but not mandatory) to use recursion to solve this problem
- You can use your favorite HTTP client library to make the API calls
- This repository is public, you don't have to worry about passing any kind of credentials in the GitHub API calls
- We would really like to see you working with `Promise` objects