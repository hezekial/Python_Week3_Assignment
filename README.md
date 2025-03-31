# Python_Week3_Assignment
def calculate_discount(price, discount_percent):
    if discount_percent >= 20:
        discount_amount = price * (discount_percent / 100)
        final_price = price - discount_amount
        return final_price
    else:
        return price

# Prompt the user to enter the original price and percentage discount
original_price = float(input("Please enter the price of the item: Ksh."))
discount_percent = float(input("Please enter the percentage discount: %"))

# Calculate the final price using the function
final_price = calculate_discount(original_price, discount_percent)

# Print the final price
if final_price == original_price:
    print("No discount applied, the final price is: Ksh.", original_price)
else:
    print("After the discount, the final price is: Ksh.", final_price)
