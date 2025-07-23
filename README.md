# ft_printf

> [!IMPORTANT]
> None of my code is publicly available here, but if you're a recruiter, I'd be happy to share it with you upon request.

<p align="center">
  <img width="317" height="268" alt="Screenshot from 2025-07-23 08-57-06" src="https://github.com/user-attachments/assets/bfae2c73-7a26-403d-acda-06b6cd9f967a" />
</p>

The ft_printf project is one of the key milestones at 42, where I had to reimplement the standard `printf` function in C. The objective was to understand how formatted output works internally — including variadic functions, string parsing, and type handling — all without using the original printf.

What I had to do:
* I implemented support for the following conversion specifiers:
  * `%c` – character
  * `%s` – string
  * `%d` / `%i` – signed integers
  * `%u` – unsigned integers
  * `%x` / `%X` – hexadecimal (lower/uppercase)
  * `%p` – pointer addresses
  * `%%` – literal percent sign
  To achieve this, I had to:
  * Parse format strings character by character
  * Use `va_list`, `va_start`, `va_arg`, and `va_end` to handle variadic arguments
  * Convert and format values correctly depending on the type
  * Manage memory efficiently and output everything using low-level functions like write
    
* Bonus Part: Extended Features
For the bonus part, I expanded ft_printf with:
  * Flags handling (like - for left-justification, 0 for zero-padding)
  * Field width and precision control
  * Handling combinations of flags, width, and precision in different orders
  * More complex formatting logic for various edge cases
This bonus section pushed my understanding further — I had to create a robust parser, manage multiple states and flags at once, and ensure proper alignment and padding behavior across all data types.

What I Learned:
* Mastery of variadic functions in C
* Parsing complex string input
* Formatting output manually without standard functions
* Handling edge cases, undefined behaviors, and precision issues
* Writing modular, maintainable, and well-tested code

ft_printf taught me how much goes on under the hood in even the simplest-looking C functions. It helped sharpen my attention to detail and boosted my confidence in handling more complex logic in pure C.
