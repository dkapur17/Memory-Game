# Memory-Game
Simple memory game where your odds of winning are 1 to 64,928,384.

To launch the game, enter into terminal:

```python3 game.py```

Don't forget to have fun!

Contributing:

I would love to expand this game and add more genres. To contribute a new genre, follow these steps:

1. Find a common genere that would be suitable for this game. Preferable one with a lot of items, but not insanely many (List of songs by Linkin Park is good. List of every english song ever, not so much).

2. Compile a .csv file of all the items from that genre with each item on a new line, and no space after the name of the item on the same line. Please try to make the list as exhaustive as possible, because the game validates the user's input based on whether or not given input is an item in the list. Also, the .csv should have atleast 50 items. Save the .csv in the CSVs directory with an appropriate name.

3. Open the game.py file and go into the ```chooseGenre()``` funtion. Here, add ```print("n. genereName")``` just above the comment ```# Add more choices here```. Replace ```n``` with the serial number and ```genereName``` with the name of the genere you're adding.

4. Just above the comment ```# Add more elif statements here``` add the following two lines:

```elif choice == "n"```
```		return csvFileName```

Replace ```n``` with the same serial number you gave above and ```csvFileName``` with the exact name that the .csv file was saved with. No need to add the extension as well.

That's about it. Now run ```python3 game.py``` and in the genre list, you should see your addition show up.