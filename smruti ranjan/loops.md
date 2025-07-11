# Loops
- Loops are used to execute a block of code  for multiple iterations.
- loops help us to execute a cotde which neads to be executed multiple times .
- there are 4 types of loops used in a coding scenario
### TYPES OF LOOPS 

<details>
<summary> For Loop </summary>

* For loop is a entry controlled loop(i.e. the conditions are cheaked before executing the block of code).
* A for loop consist of three parts which are **1.initialization 2.condition(test expression) 3.iteration expression(Iincreament/Decreament)**
	* ***initialization***
	* This sets up the loop control variable before the loop starts.
	* It is executed only once at the very beginning of the loop.

	
	* ***Test Expression/condition***
	* This is the logical test that is checked before each iteration.
	* If the condition is true, the loop continues. If the condition is false, the loop stops.
	* It is used To decide whether the loop should run again.
	
	
	* ***Iteration Expression***
	* This updates the loop control variable after each iteration.
	* It can increment (e.g., i++) or decrement (e.g., i--).
	* It is used to move the loop towards termination.
#### Example	
 ``` C#
 for (int i = 0; i < 5; i++)
{
    Console.WriteLine(i  );
}
output = 0 1 2 3 4  
```
* int i acts as the initializer
* i<5 acts as the test expression.
* i++ is the iteration expression.

 </details>

<details> <summary>while loop </summary>

* while loop is a entry controlled loop(i.e. the conditions are cheaked before executing the block of code).
* A while  loop consist of three parts which are **1.initialization 2.condition(test expression) 3.iteration expression(Iincreament/Decreament)**
	* ***initialization***
	* We must initialize the loop control variable before the while loop starts.
	* This is not part of the while loop syntax itself but is necessary for the loop to function.

	
	* ***Test Expression/condition***
	* The while loop checks this condition before every iteration.
	* If the condition is true, the loop continues. If the condition is false, the loop stops.
	* It is used To decide whether the loop should run againor terminate.
	
	
	* ***Iteration Expression (inside the loop)***
	* This updates the loop control variable after each iteration, in while loop the ieration id done inside the loop
	* It can increment (e.g., i++) or decrement (e.g., i--).
	* It is used to move the loop towards termination.

	#### Example

``` C#

int i = 0; 

while (i < 5)  
{
    Console.WriteLine("i = " + i);
    i++; 
}
output: i=0 i=1 i=2 i=3 i=4
```
* int i=0 acts as the initializer but has to be done before the loop starts.
* i<5 acts as the test expression.
* i++ is the iteration expression. which is used inside the code .

</details>

 </details>

<details> <summary>do-while loop </summary>

* Do-while loop is a exit controlled loop(i.e. the conditions are cheaked after executing the block of code).
* A do-while  loop consist of four parts which are **1.initialization 2.Loop body 3.condition(test expression) 4.iteration expression(Iincreament/Decreament)**
	* ***initialization***
	* We must initialize the loop control variable before the Do-while loop starts.
	* This is not part of the Do-while loop syntax itself but is necessary for the loop to function.
	* this happens only once and outside the loop.

	* ***Loop body***
	* The code block inside the do  is executed once, even if the condition is false.
	* After executing the block, it checks the condition.


	* ***Test Expression/condition***
	* The condition is checked after the loop body runs.
	* If the condition is true, the loop continues. If the condition is false, the loop stops.
	* It is used To decide whether the loop should run againor terminate.
	* In do-while loop the code block is executed atlest once .
	
	
	* ***Iteration Expression (inside the loop)***
	* This updates the loop control variable after each iteration, in do-while loop the ieration id done inside the loop.
	* It can increment (e.g., i++) or decrement (e.g., i--).
	* It is used to move the loop towards termination.

	#### Example
	* ***where the condition is true***
``` C#

int i = 0; 

do
{
    Console.WriteLine("i = " + i);
    i++; 
} while (i < 5); 
output: i=0 i=1 i=2 i=3 i=4
```

* int i=0 acts as the initializer but has to be done before the loop starts.
* i<5 acts as the test expression.(inside while)
* i++ is the iteration expression. which is used inside the code .


	* ***where the condition is false ***
``` C#

int i = 10; 

do
{
    Console.WriteLine("i = " + i);
    i++; 
} while (i < 5); 
output: i=10
```
* int i=10 acts as the initializer but has to be done before the loop starts.
* i<5 acts as the test expression.(inside while)
* i++ is the iteration expression. which is used inside the code .
* code is executed once befote checking the condition and then terminates.
</details>


<details><summary>Foreach loop</summary>



</details>