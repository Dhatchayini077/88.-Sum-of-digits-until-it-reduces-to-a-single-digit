# 88.-Sum-of-digits-until-it-reduces-to-a-single-digit
# Reading number
number = int(input("Enter number: "))

step = 1
while number > 9:
    total_sum = 0
    temp = number
    while temp:
        total_sum += temp % 10
        temp //= 10
    print("Step-%d Sum: %d" % (step, total_sum))
    number = total_sum
    step += 1
output
Enter number: 99999999999
Step-1 Sum: 99
Step-2 Sum: 18
Step-3 Sum: 9
