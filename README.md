## CHALLENGE 

### Challenge 1
The first challenge involved implementing a responsive animal picture gallery as shown in the provided Figma design. The objective was to ensure that the gallery is fully responsive and functions seamlessly across both desktop and mobile devices. Key features implemented included image thumbnail navigation, full-size image viewing, and interactive elements as specified in the design.

## CHALLENGE 2

### Challenge 2
The `check` function is designed to determine whether there exists a contiguous subarray within the given array `arr` that sums to the specified `target` value. To achieve this, the function uses two main variables: `start` and `currentSum`. The `start` variable marks the beginning index of the current subarray, while `currentSum` keeps the running total of the subarray elements. As the function iterates through the array with the `end` variable, it continuously adds the value of the current element `arr[end]` to `currentSum`. If `currentSum` exceeds the target, the function enters a `while` loop where it subtracts elements from the start of the subarray (using `arr[start]`) and increments the `start` index until `currentSum` is less than or equal to the target. If at any point `currentSum` equals the target, the function immediately returns `true`. If the entire array is processed without finding such a subarray, the function returns `false`. This approach ensures an efficient check for the target sum using a sliding window technique.

## CHALLENGE 3 

### Challenge 3
The `transformString` function modifies a given input string based on its length, applying different transformations depending on specific divisibility rules. The function first calculates the length of the input string. It defines two helper functions: `reverseString`, which reverses the input string, and `replaceWithASCII`, which replaces each character in the string with its corresponding ASCII code, joining these codes with spaces.

The function then checks the length of the string to determine the appropriate transformation:

- If the length is divisible by 15, it first reverses the string and then replaces each character in the reversed string with its ASCII code.
- If the length is divisible by 3 but not by 15, it simply reverses the string.
- If the length is divisible by 5 but not by 15, it replaces each character with its ASCII code.
- If none of these conditions are met, the function returns the input string unchanged.

For example, given the input "Hamburger", the length is 9, which is divisible by 3. Thus, the function reverses the string, resulting in "regrubmaH". For the input "Pizza", the length is 5, which is divisible by 5, so each character is replaced by its ASCII code, resulting in "80 105 122 122 97". Finally, for the input "Chocolate Chip Cookie", the length is 21, which is divisible by 3, so the string is reversed, resulting in "eikooCpihCetalocohC".
