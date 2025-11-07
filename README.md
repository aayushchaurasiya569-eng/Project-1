# Project-1, 
print("AAYUSH BANK".center(50,"*"))
class bank :
    def __init__(self,name,bal,ac):
        self.name= name
        self.bal= bal
        self.ac = ac
    def show(self):
        print("name :",self.name,",","balance = ",self.bal,"rs",",","account num = ",self.ac)
        print()
    def cre(self,cr):
        self.bal += cr
        print("credited amount is : ",cr,"rs")
        print()
       
    def deb(self,deb):
        self.bal-= deb
        print("Debited amount is : ",deb,"rs")
        print()
name = input("enter your name : ")
balance = int(input("enter your balance : "))
acnum = int(input("enter your account number : "))

acc = bank(name,balance,acnum)
print("---------------------------------------------------")
acc.show()
acc.cre(int(input("enter your credited amount : ")))
acc.deb(int(input("enter your debited amount : ")))
print("---------------------------------------------------")
acc.show()
