
import requests
import re


class Zeyad:
    def __init__(self):
        self.Accounts()

    def Accounts(self):
        x = int(input("ENTER ID FACEBOOK"))
        y = int(input("ENTER TARGET (1000,2000,3000)"))
        for i in range(y):
            x +=1
            a = requests.get(f"https://www.facebook.com/profile.php?id={x}").text
            b = re.compile(r'<title>(.*?)</title>', re.IGNORECASE | re.DOTALL)
            matches = b.findall(a)
            if len(matches) != 0:
                print(f"LINK : https://www.facebook.com/profile.php?id={x} \n Name : {matches}")

Zeyad()


