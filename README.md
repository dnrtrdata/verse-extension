# EduTainmental Supplementary Info for Verse

This extension provides syntax support for Epic Games' Verse programming language.

Developed by [worlds.org](https://www.worlds.org/)

This is not an official Verse VS Code extension and is not affiliated with Epic Games in any way.

##### Summarizing Epic Games' Docs on The Verse Programming Language With [Clament John's](https://github.com/clmnin) terrific *Summarize* ChatGPT extension for Chrome [so check THIS shit out - Repo ](https://github.com/clmnin/summarize.site) or [check THAT shit out - Chrome Extension Page]()

### Style Guide 
- This guide provides recommended standards for writing consistent and maintainable code.
- Adhering to these guidelines improves code readability, reduces errors, and facilitates collaboration.
- Standardized code style ensures easy understanding and maintenance by current and future developers.
- Common naming patterns are important for readable and maintainable code.
- Naming conventions include using "IsX" for logic variables, "OnX" for overloadable functions, and "SubscribeX" for framework event subscriptions.
- Avoid decorating type names and use lower_snake_case for all types.
- Interfaces should be adjectives or use "_interface" as a suffix.
- Other names should be in PascalCase, including modules, member variables, parameters, and methods.
- Parametric types should be named "t" or "thing" to represent their purpose.
- Stay consistent with formatting throughout the codebase, such as using four spaces for indentation and spaces around operators.
- Choose a formatting style that works for the project, such as using indented blocks instead of curly brackets for code blocks.
- Use explicit braces for clarity, unless compactness is necessary for the context.

- Order of operations is defined.
- Use proper spacing and formatting for brackets, identifiers, and types.
- Functions return their last expression value by default.
- Use explicit returns if necessary.
- Getters or functions with potential failure should be marked and return non-option types.
- Extension methods are preferred over single parameter methods.
- Limit the number of conditional checks/failable expressions on a single line to three.

- Use the form of if with parentheses () for fewer than three conditions.
- Use if (Damage > 10, Player := FindRandomPlayer[]) to eliminate a player.
- Keep the code concise but readable.
- Avoid splitting code over multiple lines without readability improvements.
- Use a maximum of two expressions on a single line if each expression has more than two words.
- Add a player to a team if conditions are met.
- Set player's health to 100 if conditions are met.
- Avoid complex and hard-to-parse if statements.
- Consider grouping multiple failable conditions into a single function for readability and reusability.
- Use a section comment if the code is only used in one place.
- Eliminate a player if certain conditions are met.
- Rewrite the code for getting a random player to eliminate.
- Apply the same guideline for expressions in for loops.
- Group dependent failure expressions together for better organization and readability.

---

#### Lesson 1 - Basic Programming Terms
1. Keep related conditions together to improve code locality, understanding, and debugging.
2. Group dependent or related conditions.
3. Avoid unnecessary indentation to enhance code flow.
4. Split failure contexts if handling each potential failure separately.
5. Prefer interfaces over classes to reduce implementation dependencies.
6. Use private access and restrict scope for class members and methods.
7. Postfix events with "Event" and prefix event handlers with "On".
8. Avoid decorating suspend functions with "Async".
9. Use "Await" prefix for suspends functions that wait for something to happen.
10. Put attributes on a separate line for better readability.
11. Follow import guidelines (details not provided in the text).

---
- Expressions 10.1 introduces the practice of sorting import expressions alphabetically.
- The example provided showcases import expressions for various directories.
- The directories include EpicGames.com/Temporary/Diagnostics, EpicGames.com/Temporary/SpatialMath, EpicGames.com/Temporary/UI, Fortnite.com/UI, and Verse.org/Simulation.

- Basic programming terms are essential for understanding programming.
- Familiarize yourself with prerequisite topics before proceeding.
- Verse is a programming language designed for games and simulations.
- Programs are sets of instructions that guide the computer's actions.
- Errors occur when assumptions are made instead of providing precise instructions.
- Programs need to be compiled into machine language for the computer to understand.
- Algorithms are sets of instructions that solve problems or accomplish tasks.
- Algorithms can involve loops, which repeat instructions until stopped.
- Fortnite Creative utilizes algorithms to create game mechanics.
- Verse programming allows for the conversion of algorithms into computer instructions.
- Testing algorithms is important to ensure they function as intended.

- Algorithm for making tea or coffee:
1. Write out the algorithm for brewing the drink.
2. Follow the algorithm precisely.
3. Taste the brewed tea/coffee to determine if it's good to drink.
4. If it's good, the algorithm is done. If not, debug the steps to identify errors.
5. Iterate and make design changes until you achieve the perfect cup.

- Source code and machine code:
- Source code is the program written by a programmer, representing the original version.
- Machine code is the compiled version of the program that the computer can understand.

- Execution:
- When a computer runs or executes a program.

- Errors in code:
- Compiler errors: Code fails to compile into a language the computer can understand.
- Bugs: Code compiles successfully, but the program doesn't run as expected.

- Compiler errors:
- Common cause: Incorrect syntax.
- Syntax defines the rules for combining words and symbols in a programming language.
- Syntax includes the permissible words, symbols, and their arrangement.
- Case sensitivity and proper spacing are crucial in syntax.

- Bugs:
- Occur when the program executes but behaves unexpectedly.

Note: The text seems to be cut off mid-sentence. If there's more content, please provide it, and I can continue summarizing.

- Semantics in programming refers to the meaning of code, while syntax refers to the rules of writing code.
- Errors in code meaning can lead to bugs in a program.
- The example code demonstrates a bug where the condition for winning is incorrectly set to MiceCaught > 1 instead of MiceCaught > 0.
- Programs instruct computers on input and output using compiled human-readable source code.
- Algorithms provide a model for how a program should function.
- Source code is readable by humans, while machine code is executable by computers.
- Compiler errors prevent program compilation, while bugs occur when compiled code doesn't run as expected.

##### Summarizing with an informal combination of inline-code and table formatting 'cuz I like tables :), but I don't trust Markdown... :( to format them better than I can when immplementing irrisponsible time-wasting... :)) tick tik tok :((

### Ver(se)nacular:

A:

B:

C:
  - Code Comments

``` DrawingCodeWithPreciousWordses_AndCommentsesingWithPunctuationses
|-------------------------------------------------------------------------------------------------------------------------|
| 1+2 # Hola MukthaFkcka! | SINGLE-LINE COMMENT (^1) |
|-------------------------------------------------------------------------------------------------------------------------|
| 1<# inline comment, yo! #>+2 | INLINE BLOCK COMMENT: Anything appearing btwn <# and #> is part of the inline block-comments can be betweeen expressions on a single line and don't change the expressions. |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| DoDis_Homie() <# And they can run multpl long lines #> DatHomie() | MULTI-LINE BLOCK COMMENT: Anything that appears betweeen <# and #> is part of the code comment. (^2) |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <# Block comments nest <# like this #> #> | NESTED BLOCK COMMENT: Anything that appeasrs btwn <# and #> is part of the code comment. (^3) |
|-----------------------------------------------|

(^1) Anything btwn # and the end of the line is part of the code comment.
(^2) Multi-line block comments can span multiple lines.
(^3) This can be useful if you want to comment out some expressions in a line for testing and debugging without changing an existing code comment. Verse be taking code-comments seriously. I'm sincerely endeared to it for this. Fo real.
```

### Constants

``` DrawingWithPreciousWordses_AndConstantPunctuationses
|--------------------------------------------|
| Declaration               | Initialization |
|--------------------------------------------|
| Identifier,           Type |Expression     |
| MyF'ingConstant  , :, float|=, 2.0         |
|--------------------------------------------|
```
D:
E:
F:
G:
H:
I:
J:
K:
L:
M:
N:
O:
P: 
### Variables

