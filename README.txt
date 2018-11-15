Setup: (Complete)
In DFA TM begins by appending 1C right before the input tape.
The 1 represents q0 the intial vertice and C means it's right before current input.

Z will be the symbol for the start of the stack
left of Z we be stack going up.

For DPDA TM Appends 1Z1C before the input tape.
1Z is the stack with only Z in it.
----------------------------------------------------------------------------------------------------
fnd_state:(Complete)

In the DFA TM this marked the intial 1 to X and went through and marked every qi after D to x. 

Adjusted for new symbols
------------------------------------------------------------------------------------------------------
fnd_input:(Complete)

In the DFA block this went through and marked the n to y.
This works for now. Might have problems a few iterations in though
------------------------------------------------------------------------------------------------------
fnd_pop:(Incomplete):

Have to mark as read with r then go and check the stack. 
Ends at C
-------------------------------------------------------------------------------------------------------
fnd_write:(Incomplete):

In the DFA block this went through and marked the qj to z

-------------------------------------------------------------------------------------------------------
wrt_push:(Complete):

Go through and mark all read push symbols as s then push onto stack.
Ends at C
-------------------------------------------------------------------------------------------------------
reset:(Incomplete):

Go through the tape and reset everything back to normal except for consumed input and stack.
--------------------------------------------------------------------------------------------------------