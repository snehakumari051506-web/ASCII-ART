# ASCII art of Dan Brown
def draw(ch, no):
    char = ""
    index = 0
    while index < no:
        char += ch
        index += 1
    return char

    def row1():
    # Top of head/hairline
   string = ""
  string += draw(" ", 25)
  string += draw("@", 30) # Dense character for dark hair
    string += draw(" ", 25)
    return string

def row2():
    # Forehead area
    string = ""
    string += draw(" ", 20)
    string += draw("%", 40) # Medium density for skin texture
    string += draw(" ", 20)
    return string

def row3():
    # Eye line - using # for higher contrast
    string = ""
    string += draw(" ", 18)
    string += draw("#", 8)   # Left Eye
    string += draw(" ", 18)
    string += draw("#", 8)   # Right Eye
    string += draw(" ", 18)
    return string

def row4():
    # Nose and cheekbones
    string = ""
    string += draw(" ", 38)
    string += draw("+", 4)   # Highlights for the nose
    string += draw(" ", 38)
    return string

def row5():
    # Mouth and chin
    string = ""
    string += draw(" ", 30)
    string += draw("=", 20)  # Moderate density for the jawline
    string += draw(" ", 30)
    return string

    # List of all row functions
functions = [
    row1,
    row2,
    row3,
    row4,
    row5
]

# Print the final portrait to the terminal
print("Generating Dan Brown ASCII Portrait...")
for func in functions:
    print(func())
    
