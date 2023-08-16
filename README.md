# CloneTrader
"CloneTrader" Copy Trading Bot Project: This Python script utilizes the API to perform copy trading in financial market. It continuously fetches currency prices, calculating Risk management configurations. 
Here's what the main execution part of the code does:
•	It retrieves the open positions from the master account using master_api.list_positions().
•	It fetches the client account's portfolio equity using client_api.get_account() and converts it to a floating-point number.
•	It iterates through each position in the master account and calculates the maximum allowed position size based on the risk management configuration.
•	If the position's market value is within the allowed size, it submits an order to open the same position in the client account.
•	If the position's market value exceeds the allowed size, it prints a message indicating that the position is skipped due to excessive risk.
If any errors occur during the process, they are caught and handled with appropriate error messages

