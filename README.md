# Based on a user's order, work out their final bill.
# Small pizza (S): $15
#Medium pizza (M): $20
#Large pizza (L): $25
#Add pepperoni for small pizza (Y or N): +$2
#Add pepperoni for medium or large pizza (Y or N): +$3
#Add extra cheese for any size pizza (Y or N): +$1 #


print("Thank you for choosing Python Pizza Deliveries!")
# What size pizza do you want? S, M, or L
size = input("What size of pizza do you want? \n"+"Answers below - either S=Small or M=Medium or L=Large\n")

bill=0

if size == "S":
    bill += 15
elif size =="M":
    bill += 20
else:
    bill += 25
# Do you want pepperoni? Y or N
add_pepperoni = input("Do you want pepperoni? \n"+"Answers below - either Y=Yes or N=No\n")

if add_pepperoni =="Y":
    if size =="S":
        bill += 2
    else:
        bill += 3

# Do you want extra cheese? Y or N
extra_cheese = input("Do you want extra cheese? \n"+"Answers below either Y=Yes or N=No\n")

if extra_cheese == "Y":
    bill += 1
else:
    bill += 0

print(f"Your final bill is: ${bill}.")





