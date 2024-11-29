WHEN ANALYING A SINGLE GATE BY ITSELF:
A 0 on both inputs always leads to a 0 output.
- The (1, 0) and (0, 1) columns produce the same output.
	- However an exception to this is a 0 on a not gate will invert this.


A bubble, indicates that it is low active, (active low) 

When things happen they will go low, (active low, it will actively do something when low


Memorize the distinct shape of each gate




Each gates has a unique <u>truth table</u>.

# AND
An AND gate produces a 1 output if and only if all of its inputs are 1.
- Associate a AND gate with multiplication.
# OR
An OR gate produces a 1 if and only if one or more of its inputs are 1.
- Associate A OR gate with addition.
# NOT
A NOT gate, usually called an inverter, produces an output value that is the
opposite of its input value.


- A NOT gate is basically a buffer gate with a circle too.

Compliment can be represented by a prime symbol or a top bar.

A NOT gate turns $a$ into $a\prime$ and vice versa.

$$
a\prime\hspace{3em}\overline{a}
$$
$$
0\prime=1\; \hspace{1em}\&\hspace{1em} 1\prime=0
$$
# NAND
A NAND gate produces the opposite of an AND gate’s output, a 0 if and
only if all of its inputs are 1


# NOR
A NOR gate produces the opposite of an OR gate’s output, a 0 if and only
if one or more of its inputs are 1.




# Latch



# Simple Flip Flop
- The key feature of a flip-flop is its ability to maintain its state (either 0 or 1) until it is changed by the inputs. 
	- With this kind of circuit is is possible to capture memory of the past.


- A flip flop can be constructed in two different ways.
	- One is a simple way (Below is shown the simple way).
	- The other way based on a latch design with an additional control input.


Here the output is a function of the input and output, since we can see a connection going from the output back into the AND gate. 

![[Logic Gates-20240909152958505.webp|535]]

| A (Input 1) | B (Input 2) |  C  |  D  |  E  |
| :---------: | :---------: | :-: | :-: | :-: |
|      0      |      0      |     |     |  0  |
|      0      |      1      |     |     |  0  |
|      1      |      0      |  0  |  0  |  X  |
|      1      |      1      |     |     |  X  |


Explanation of operation:
### Initial State
- Initial State: Both inputs are 0, and let’s assume the output is off.

### Turning on(setting)
- Turning On: When you press the upper input (set it to 1), the OR gate gets a 1, making its output 1. This 1 goes to the AND gate, which also gets a 1 from the NOT gate (since the lower input is 0). So, the AND gate’s output becomes 1, which feeds back into the OR gate, keeping its output at 1.

Setting the output to 1: (<u>quick pulse</u> to input A)
A:1 
B:0

Changing to this will keep the output to 1. This keeps the same output as before. (depends on previous input). As long as both inputs in the circuit remain 0, the output (whether 0 or 1) will not change.

### Maintaining State
Maintaining State: Now, even if you release the upper input (set it back to 0), the OR gate still has a 1 from the AND gate. This keeps the AND gate’s output at 1, maintaining the OR gate’s output at 1.
A:0
B:0


### Turning off(resetting)
Reset: Output 0
A:0
B:1


# SR (Set-Reset)