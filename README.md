# Simple-stock-codealpha
stocks = {
    "AAPL": 180,
    "TSLA": 250,
    "GOOGLE": 150
}

total = 0

print("Stock Portfolio Tracker")

while True:
    name = input("Enter stock name (or DONE): ").upper()

    if name == "DONE":
        break

    if name in stocks:
        qty = int(input("Enter quantity: "))
        total += stocks[name] * qty
    else:
        print("Invalid stock")

print("Total Investment =", total)

