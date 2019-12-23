# listperfectno
To list all perfect numbers
""" This script will list all perfect numbers with in th input variable
    If user has given variable as 100, it will list all perfect numbers in the range of 1-100"""
class listperfectno() :
    def __init__(self, a):
        self.a = a
    def permodule(self):
        # c = 0
        # flag = 0
        d = self.a
        while (d != 1 ) :
            c = 0
            flag = 0
            for i in range(1, self.a):
                if self.a % i == 0:
                    c += i
            if self.a == c:
                print(self.a, "IS A PERFECT NUMBER !!")
            # else:
            #     print(self.a, "Not a perfect no")
            self.a -= 1
            d -= 1

var1 = listperfectno(100000)
var1.permodule()
