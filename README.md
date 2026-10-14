# C--program10

# Understanding the Return Value of `scanf()` in C

## 1. Description
This C program accepts an integer from the user using `scanf()` and displays the return value of the function.

The return value indicates how many input items were successfully read and assigned.

## 2. Algorithm
1. Start.
2. Declare two integer variables, `ret` and `no`, and initialize them to `0`.
3. Ask the user to enter a number.
4. Read the number using `scanf()` and store its return value in `ret`.
5. Display the value of `ret`.
6. Terminate the program using `EXIT_SUCCESS`.

## 3. Concepts Used
- `scanf()` function
- Return values
- Integer variables
- `printf()` function
- `EXIT_SUCCESS`
- Header files: `stdio.h` and `stdlib.h`

## 4. Sample Output

**Example 1: Valid integer input**

```text
Enter number :
25
Return value is : 1
```

**Example 2: Invalid integer input**

```text
Enter number :
abc
Return value is : 0
```

## 5. Explanation
- **Return value `1`:** One input item was successfully read and assigned.
- **Return value `0`:** The input did not match the expected integer format.
- **Return value `EOF`:** The input failed before the first conversion could occur because the input stream reached its end or encountered a read error.

In this program, `scanf("%d", &no)` expects an integer.

## 6. Compilation and Execution

Compile using GCC:

```bash
gcc program.c -o program
```

Run on Windows:

```bash
program.exe
```

Run on Linux/macOS:

```bash
./program
```

## 7. Conclusion
This program demonstrates how the return value of `scanf()` can be used to determine whether the expected input was successfully read. For one integer conversion, a return value of `1` indicates success.
