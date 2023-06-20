# Zombie-Congaline
C++ data structures project for CSE240 with Professor Justin Selgrad. 

Program info:
    Congaline is a templated linked list populated with Zombie objects. Zombies can be Red, Yellow, Green,
    Blue, Magenta and Cyan. termcolor.hpp will color the zombies' output text to match their color. Every turn will randomly generate a Zombie object and perform a random action on it. 
    Actions include: 
      Engine! 
        This zombie becomes the first Zombie in the conga line
      Caboose! 
        This zombie becomes the last zombie in the conga line
      Jump in the Line! 
        This zombie joins the conga line at position X where X <= length of the linked list
      Everyone Out! 
        Remove all matching zombies from the linked list
      You Out! 
        Remove the first matching zombie from the linked list
      Brains! 
        Generate two more matching Zombies and add one to the front (engine_action), one to the end (caboose_action) and one to the middle (round down).
      Rainbow Brains! 
        Perform an engine_action on the zombie that was generated. Add one of each zombie color to the end via caboose_action in this order: Red, Yellow, Green, Blue, Cyan, Magenta
      Making new Friends! 
        Find the first Zombie of this color in line. Do a coin flip – if rand() % 2 == 0 then insert before, else insert after. If no Zombie of that color exists, then perform caboose_action on the zombie

Running the program:
    Run the makefile in the project directory. The makefile will create an executable named "exe"
