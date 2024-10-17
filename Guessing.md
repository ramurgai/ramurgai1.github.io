```mermaid
flowchart TD
Start([Start]) --> A(Program generates a 
random number 0-9)
A-->B(The program prompts the
 user for input)
B-->C[/The user enters a number/]
C-->D(The number is checked)
D-->E(The number is correct)
E-->End([End])
D-->F(The answer is not correct)
F-->G(The program prompts the 
user to see if they would 
like to continue with the 
game)
G-->H[\The user enters yes or no\]
H-->I(They choose no)
H-->J(They choose to continue)
J-->C
I-->End([End])

```
## Explanation:
So basically the thing starts with the program creating the number, 
then the person will be prompted for a number, 
they enter a number, 
the program checks to see if it's right, 
if it's right then the thing ends, 
if it isn't then they can either choose to continue or they can quit,
if they chose to quit then the thing ends, 
if they choose to continue then they go back to the point where they enter a number and the process repeats until they quit or guess the number correctly.