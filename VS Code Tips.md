- How to run multiple different programs with their own main method inside the same project/folder in VS code? Is it looking for directly for the `Main` function? So is this why it complains if there is multiple Main functions?
	- Yes 
	- Hello



# Debugger
- When I try to run the debugger, the step over, step into, and step out options are greyed out and not able to click them?
	- You have to put at least one break point.




### How Does a Breakpoint Work?
1. Set a Breakpoint: When you’re writing code in an environment like Visual Studio Code, you can click on the margin next to a line number to set a breakpoint. A red dot will appear, marking where you want the program to pause.
2. Run the Program: When you run your program with a debugger (a special tool that helps you look into your code as it runs), the program will start normally.
3. Hit the Breakpoint: When the program reaches the line where you placed the breakpoint, it pauses. It’s like a remote control for your code where the breakpoint is your "pause button."
4. Inspect the Program: While the program is paused at the breakpoint, you can:
	1. See the values of variables at that exact moment.
	2. Step through the code line by line to see what happens next.
	3. Check how the program is behaving up to that point.


> [!Info] By setting a breakpoint, you’re telling the computer:
> Stop running the program when you reach this line, so I can take a closer look.


How to know which option to choose? (step over, step into, step out)?

Once the program is paused, you can do a few things:
- Step over: Move to the next line of code and see what happens there.
- Step into: If there’s a function call, you can go inside that function to see how it works.
- Step out: If you're inside a function and want to leave it, you can step out back to where it was called.
- Continue: If you’re done inspecting, you can let the program continue running as usual.
