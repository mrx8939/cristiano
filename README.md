# cristiano
# i want to develop this program
import time
x1 = input("""             sing up
   enter your username: """)
x2 = input('   password khod ra vared konid: ')
x3 = input("""             log in
    enter username for log in: """ )
x4 = input('    enter password for log in: ')

if x3 != x1 or x4 != x2:
    print('pass ya username eshtebah ast.')
    exit()
    
if x3 == x1 and x4 == x2:
    print('*******khosh amadid*******')      
        

def main():       
    time.sleep(1)
    x = input("""
    ***menu***

    mikhaid chikar konid?

    enter B baraye mashin hesab >

    enter C baraye bazi hads adad >

    enter Z baraye tamas ba ma >""")



    pq = ['A','a','B','b','C','c','Z','z']
    if x not in pq:
        print('lotfan icon dorost ra entekhab konid')
        exit()


    def tamas1():
        if x == "Z" or x == "z":
            print("""telefon ma: 09365419527
        id telegram: @wsrcm""")
            b1 = input("""*************

enetr Y baraye bargasht be menu
enter har harfi baraye exit: """)
            if b1 == 'Y' or b1 == 'y':
                main()
            else:
                exit()
    tamas1()
        
     
        
    def mashin_hesab2():
        if x == 'B' or x == 'b':
            print('***mashin hesab***')
            x1 = int(input('adad aval?'))
            x2 = input('- + * / ? ')    
            x4 = int(input('adad dovom?'))

            if x2 == '-':
                x5 = x1 - x4
                print(x5)
            if x2 == '+':
                x6 = x1 + x4
                print(x6)
            if x2 == '*':
                x7 = x1 * x4
                print(x7)
            if x2 == '/':
                x8 = x1 / x4
                print(x8)
            b2 = input("""*************

enetr Y baraye bargasht be menu
enter har harfi baraye exit: """)
            while True:
            if b2 == 'Y' or b2 == 'y':
                main()
            if b2 == 'N' or b2 == 'n':
                exit()

    mashin_hesab2()








    def hads_adad3():
        if x == 'C' or x == 'c':
            import random

            print('***hads adad az 1 ta 15 hads bezan***')

            x1 = random.randint(1,15)

            while True:
                x2 = int(input('hadset?'))

                if x2 > x1:
                    print('adad kochik tare')
                if x2 < x1:
                    print('adad bozorg tare')
                if x2 == x1:
                    print('***bordy***')
                    exit()
    hads_adad3()
        
    exit()

main()





