# Function.16
Two players, Nikhil and Babu, take turns subtracting either 10 or 20 from a starting number.
def player_Nikhil(n):
    if n<=0:
        print("player Nikhil reached 0!! player Nikhil loses")
        return
    print(f"\n player Nikhil's trun. Current number{n}")
    move = int(input("player Nikhil, subtract 10 or 20:"))
    while move not in[10,20]:
        move = int(input("player Nikhil, subtract 10 or 20:"))
    player_Babu(n-move)
def player_Babu(n):
    if n<=0:
        print("player Babu reached 0!! player Babu loses")
        return
    print(f"\n player Babu's trun. Current number{n}")
    move = int(input("player Babu, subtract 10 or 20:"))
    while move not in[10,20]:
        move = int(input("player Babu, subtract 10 or 20:"))
    player_Nikhil(n-move)
start = int(input("enter a number:"))
player_Nikhil(start)
