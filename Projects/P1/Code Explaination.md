## Creating the start menu:
1. Start in program.cs
2. Enter startmenu.cs `StartMenu start = new();`
	1. Create the world map
	2. Print the world map 
3. Enter messages.cs
	1. Print the start message.
4. Go back to startmenu.cs
	1. Print the “press any key to continue”
	2. Print “please enter the name of your city”

## Create a player, which has an inventory:
5. Enter game.cs `Game game = new(start.CityName);`
	1. Enter the constructor `public Game(string cityName)`
6. Enter Inventory.cs `_player = new Player(new Inventory(this));`
	1. Enter the constructor `public Inventory(Game game)`
7. Enter Item.cs `Item item = new Item("Showel", "Nice showel", "dig a hole", 500);`
8. Go back to game.cs
	1. Enter: `private void CreateRooms(string mainCityName)

## Creating the locations:
9. Enter manilla.cs ``
	1. Enter the constructor `public Manilla(Game game, Player player) : base("Manilla")`
	2. Enter location.cs
10. Go back to 
	1. Enter SampleSpecificLocation.cs

## Playing the game:
11. Go back to Program.cs
12. Enter game.cs `game.Play();`
	1. Enter `public void Play()`
	2. Print the welcome message
	3. Print the help message
13. Inside game.cs go to the ChangeCurrentLocation Method `ChangeCurrentLocation(TravelMenu);`
	1. Go to TravelMenu.cs `CurrentRoom.Play();
14. Inside TravelMenu.cs, print the start message (which location to pick) `DisplayStartMessage();`
	1. Get Input
15. Go to parser.cs to check the input.
16. Go to command.cs
17. Go to commandexecuter.cs
	1. Run `ExecuteTravel()`
18. Go to game.cs
	1. Run `ChangeCurrentLocation(Location location)`
`






Player has an inventory and items belong in the inventory.


# CommandLogic
## Command.cs

## CommandExecuter.cs

## CommandWords.cs

## Parser.cs
- Parser for each set of command words

# InventorySystem
## HappinessIndicator.cs

## Inventory.cs
- Currency and physical items are items in the inventory.

## InventoryItem.cs

## Item.cs

## NPC.cs

## ShopItem.cs

# Maps

# Messages

## Messages.cs
Messages are all stored in this file and are accessed using a switch case.

# Main Directory:

## Game.cs

## Player.cs

## Program.cs

## StartMenu.cs












Flow of execution:
1. 