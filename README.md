# stone_paper_game_rudhram
code 

<!-- start code -->

import random
i = ["s","p","sc","q"]
c = 0
y = 0
d = 0
name = input("enter your name : ").upper()
while True:
        k = random.randint(0,2)
        
        print("enter s (for stone) or p (for paper) or sc (for scissors) or q (for quit)")
        inp = input().lower()

        if inp=='q':
            quit() 
        elif inp not in i:
            print("please enter valid case!")
            continue
        elif i[k]==inp:
            print("draw!")
            d+=1
            continue
        elif inp=='s' and k==1 :
            c+=1
            print("you loss")
            continue
        elif inp=='p' and k==2:
            c+=1
            print("you loss")
            continue
        elif inp=='sc' and k==0:
            c+=1
            print("you loss")
            continue
        else:
            y+=1
            print("you won")
    
            print("\n\n--final score--\n")
            print("COMPUTER",name,"DRAW","\n",c,"       ",y,"     ",d)
            
<!--       end code      -->
