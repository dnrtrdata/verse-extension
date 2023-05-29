# Syntax Support for Verse

This extension provides syntax support for Epic Games' Verse programming language.

Developed by [worlds.org](https://www.worlds.org/)

This is not an official Verse VS Code extension and is not affiliated with Epic Games in any way.

## Summarizing Epic Games' Docs on The Verse Programming Language With [Clament John's](https://github.com/clmnin) terrific *Summarize* ChatGPT extension for Chrome [so check THIS shit out - Repo ](https://github.com/clmnin/summarize.site) or [check THAT shit out - Chrome Extension Page]()

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

Here are the summarized bullet points based on the provided text:

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

- Expressions 10.1 introduces the practice of sorting import expressions alphabetically.
- The example provided showcases import expressions for various directories.
- The directories include EpicGames.com/Temporary/Diagnostics, EpicGames.com/Temporary/SpatialMath, EpicGames.com/Temporary/UI, Fortnite.com/UI, and Verse.org/Simulation.

## Summarizing with tables 'cuz I like tables :)
# Ver(se)nacular:

## C:

### Comments

``` DrawingWithPreciousWordses_AndPunctuationses
|-----------------------------------------------|
| 1+2 # Hola MukthaFkcka! | single-line comment: Anything btwn # and the end of the line is part of the code comment. |
|--------------------------------------------------------------------------------------------------------------------|
| 1<# inline comment, yo! #>+2 | inline block-comment: Anything appearing btwn <# and #> Inline block-comments can be betweeen expressions on a single line and don't change the expressions. |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| DisHomie() <# And they can run multpl long lines #> DatHomie() | Anything that appears betweeen <# and #> is part of the code comment. Multi-line block comments can span multiple lines. |
|-----------------------------------------------|
| <# Block comments nest <# like this #> #> | nested block comment: Anything that appeasrs btwn <# and #> is part of the code comment. This can be useful if you want to comment out some expressions in a line for testing and debugging without changing an existing code comment. Verse be taking code-comments seriously. I'm sincerely endeared to it for this. Fo real. |
|-----------------------------------------------|

### Constants

``` DrawingWithPreciousWordses_AndPunctuationses
|--------------------------------------------|
| Declaration               | Initialization |
|--------------------------------------------|
| Identifier,           Type |Expression     |
| MyF'ingConstant  , :, float|=, 2.0         |
|--------------------------------------------|
```

## Variables

