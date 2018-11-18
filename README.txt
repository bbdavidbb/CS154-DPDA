Pretty much done.

Changed the stack to the back of the input string because saving current state and 
doing stack operations in the same area lead to a lot of bugs.

Added a bunch of other blocks to handle like clean_up to handle edge cases and 
fit with the flowchart.
---------------------------------------------------------------------------------------------------
Setup: (Complete)
In DFA TM begins by appending 1C right before the input tape.
The 1 represents q0 the intial vertice and C means it's right before current input.

T will be the symbol for the start of the stack
right of T will be the stack

For DPDA TM Appends 1C before the input tape.
and appemds T1 to the end of the stack.
----------------------------------------------------------------------------------------------------
fnd_state:(Complete)

In the DFA TM this marked the intial 1 to X and went through and marked every qi after D to x. 

Adjusted for new symbols
------------------------------------------------------------------------------------------------------
fnd_input:(Complete)

In the DFA block this went through and marked the input char to y.
------------------------------------------------------------------------------------------------------
fnd_pop:(Complete):

Have to mark as read with r then go and check the stack.
If matches pop off the stack. 
-------------------------------------------------------------------------------------------------------
clean_up:(Complete)

Changes any D transitions to N if they don't meet transition conditions
-------------------------------------------------------------------------------------------------------
wrt_state:(Complete):

In the DFA block this went through and changed current state to transitioned state
-------------------------------------------------------------------------------------------------------
wrt_push:(Complete):

Go through and mark all read push symbols as s then push onto stack.
-------------------------------------------------------------------------------------------------------
reset:(Complete):

Go through the tape and reset everything back to normal except for consumed input and stack.
--------------------------------------------------------------------------------------------------------
chk_trans:(Complete)
From the DPDA flowchart.
-------------------------------------------------------------------------------------------------------
chk_csm:(Complete)
From the DPDA flowchart.
-------------------------------------------------------------------------------------------------------
chk_final:(Complete):
Check if current state is a final state. 
--------------------------------------------------------------------------------------------------------
reject:(Complete)
--------------------------------------------------------------------------------------------------------
accept:(Complete)