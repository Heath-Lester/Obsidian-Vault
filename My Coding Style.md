
In accordance to limited focus theory, you write so that when reading code what is in your focus, or RAM as it were, is the least amount of information necessary to understand. 

This means that things like common errors or edge cases are handled as early as possible or is at the top of the code block so that when reading the remaining logic things that do not need to take up focus are not necessary to keep in mind.

- If it can be handled earlier, it should. Code "aesthetics" are secondary.
- Store what is needed for a section of logic above where it started to be used or handled.
- Logic should always be at the bottom
- In the logic section "administrative" logic, assigning, reassigning variables used to evaluate should be placed above "handling" logic
- "handling" logic should be placed last

*It seems as if in the majority of efficient algorithms I create, the "administrative" logic tends to be at the end as opposed to when I create brute force solutions it tends to be at the beginning.