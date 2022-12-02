**Car loan payments.** Write a program CarLoan.java that reads in three command-line arguments P, Y, and R and calculates the monthly payments you would have to make over Y years to pay off a P dollar loan at R per cent interest compounded monthly. The formula is The formula is:
````
                P r 
payment =  ---------------,  where n = 12 * Y, r = (R / 100) / 12
           1  - (1 + r)^(-n)
````
