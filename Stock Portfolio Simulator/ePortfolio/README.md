1) This code is a stock portfolio simulator which holds stocks of two different types mutualfund and stock. The main should be included in the porfolio class which within porfolio i have added more methods to maintain 2 arrays of different types: stock and mutualfund and updating selling and buying investments
2) I assume that I will only have my mutator and accesor methods, any gain related, or payment related methods in my stock and portfolio classes. All methods 1-5 in the assignment description should go in my portfolio class and in that class I will have my methods which work on the lists themselves performing actions such as: selling, buying, updating, or getting gain of all the investments. My limitations will be performance. Despite the inneffiecency of doing all methods twice or having a portion for both stock and mutual fund classes in each method, I know that our next assignment is to utilize inheritance and optimize my code more making it much more effiecent then I am able to in this project. Another is that I cannot integrate real time market data for stocks and will need to rely on user inputs for price updates.
3) 
build: javac ePortfolio/*.java 
test: java ePortfolio.Portfolio
buy: buys stock or mutual fund based on user inputs 
sell: sells stock or mutual fund based on user inputs 
update:  updates the price of all existing investments based on user inputs
getgain: no input required will get gain if you were to sell all existing investments
search: Based on user inputted fields will match investments to specific ranges keywords or symbol
4) test plan:

Menu case 1: Invalid menu option (e.g., typing a number outside the valid range).
Input: Enter an invalid option.
Expected Result: Error message: “Invalid choice. Please try again.”
Menu Case 2: Enter an empty menu input and check system behavior.
Input: Enter an empty option (blank input).
Expected Result: Error message: “Please select a valid option.”

buy: 
- buy 500 aapl stock
- buy 300 more aapl stock at 100$ both
- try buying with negative value should print error handling

sell: 

- try to sell more than you own should print error handling
- Sell fully make sure investment is deleted
- try to sell negative value should error handle

update:

- update and make sure all prices are refreshed
- update with negative values
- update empty list 

getgain:

- get gain of empty list
- get gain of mixed mutual funds and stocks make sure values are correct

search:

- search for each case/combination of possible inputs eg. only symbol only price only keywords test every mix between them and test empty input for each field
Test Case 1:

Input: Choose "Search", enter symbol = "", keywords = "tech", priceRange = "".
Expected Result: System returns all investments with the keyword "tech" in the name.
Test Case 2:

Input: Choose "Search", enter symbol = "", keywords = "", priceRange = "50-200".
Expected Result: System returns all investments within the price range $50 to $200.
Test Case 3:

Input: Choose "Search", enter symbol = "AAPL", keywords = "tech", priceRange = "".
Expected Result: System returns all AAPL investments with the keyword "tech" in the name

Expected Output: Error message for invalid numeric input.
5) If i had more time and could do the assignment again I would have used documentation more throughout my coding process because going back and reading large functions trying to trace through difficult to understand code took up alot of time. I would also refactor large methods like search and buy further so that they are more manageable and using small helper functions would allow for better readability. Lastly I would add a bit more error handling and defensive programming to ensure no crashes would occur. 