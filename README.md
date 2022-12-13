# codes
print("CURRENCY CONVERTOR".center(189,'-'))
print("LIST OF CURRENCIES: ")
print("INR-Indian rupee \t\t GBP-British Pound sterling")
print("EUR-Euro \t\t\t\t USD-US dollar")
print("CAD-Canadian Dollar \t CNY-Chinese Yuan")
print("RUB-Russian Ruble \t\t AED-Arabic dirham")
print("LKR-SriLanka rupee \t\t NZD-New Zealand dollar")
list_of_currencies =
['INR','GBP','EUR','USD','CAD','CNY','RUB','AED','LKR','NZD']
input_curr = input("Enter the source currency: ")
output_curr = input("Enter the target currency: ")
while(input_curr not in list_of_currencies or output_curr not in
list_of_currencies):
 if(input_curr in list_of_currencies and output_curr not in
list_of_currencies):
 print("{} is not in the list of Currencies..Try
Again!".format(output_curr))
 elif(input_curr not in list_of_currencies and output_curr in
list_of_currencies):
 print("{} is not in the list of Currencies..Try
Again!".format(input_curr))
 else:
 print("Both {} and {} are not in the list of Currencies..Try
Again!".format(input_curr,output_curr))
 input_curr = input("Enter the source currency: ")
 output_curr = input("Enter the target currency: ")
rate = eval(input("Enter the Conversion rate: "))
amount = eval(input("Enter the amount in {}: ".format(input_curr)))
final_amount = "{0:.2f}".format(rate*amount)
print("{} {} is {} {}".format(amount,input_curr,final_amount,output_curr))
