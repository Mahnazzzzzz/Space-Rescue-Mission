print('''
                    oooooOOOOOOOOOOOOOOOOooooo
                  AAAAAAAAAAAAAAAAAAAAAAAAAAAAAA
                 IIIIIIIIIIIIIIIIIIIIIIIIIIIIIIII
                HHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHH
               zzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzz
    .<><><><><><><><><><><><><><><><><><><><><><><><><><><><>.
  /XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX/
/XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX/
\XXX[  ]XXX[  ]XXXX[  ]XXXX[  ]XXXX[  ]XXXX[  ]XXXX[  ]XXX[  ]XXX/
  \XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX/
      ~~~~\XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX/~~~~
               /   ~~~<><><><><><><><><><>~~~     /
              /      /       |   |          \      /
             /     /               |          \     /
            /    /           |                  \    /
           /   /               |   |              \   /
          /  /               |                      \  /
        _/_/                     | |                  \_\_
       <___>                 |    |                   <___>
                                    |
                              |

''')

print("Welcome to Space Rescue Mission.")
print("Your mission is to rescue stranded astronauts on a distant planet.")

direction = input("You are at a cross road. Where do you want to go? type left or right. ")

if direction == "right":
    print("You've reached an unknown planet.")

decision_1 = input("Do you leave the spaceship or land on the planet? type leave or land. ")

if direction == "right" and decision_1 == "land":
    print("You've safely landed on the planet.")
elif direction == "right" and decision_1 == "leave":
    print("An alien ate you. Game Over!")

decision_2 = input("You see astronauts running toward your spaceship. Do you leave the spaceship and run toward them or wait? type leave or wait. ")

if direction == "right" and decision_1 == "land" and decision_2 == "wait":
    print("You see they are being followed by aliens")
elif direction == "right" and decision_1 == "land" and decision_2 == "leave":
    print("A disgusting alien ate you. Game Over!")

decision_3 = input("The astronauts reach the spaceship. Do you open the door or keep it close? type open or close. ")

if direction == "right" and decision_1 == "land" and decision_2 == "wait" and decision_3 == "open":
    print("Congratulations! You've rescued the stranded astronauts. You Won!!")
elif direction == "right" and decision_1 == "land" and decision_2 == "wait" and decision_3 == "close":
    print("the stranded astronauts were eaten by the aliens and their blood splashed on your spaceship selfish bastard :| Game Over!")
else:
    print("You fell into a black hole. Game Over!")
