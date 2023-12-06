Staircase Time Complexity:

Staircase Space Complexity:

Alternating Characters Time Complexity: The time complexity is O(n) because the function processes each 
character in the string once, resulting in a number of operations linearly proportional to the length of the input string.

Alternating Characters Space Complexity: The space complexity is also O(n) because the amount of calls is related 
to the length of the string. We can check each letter to see if it is required to delete
the character or not and we keep track of that with the "del" variable. Since we make a recursive call each letter
we end up with a O(n) space complexity.

Alternating Characters Recurssive definition:

Base case: If the string has one or fewer characters, no deletions are needed, so the function returns 0.

Recursive case: If the current character is the same as the next one, we increment the deletions by 1 and recursively 
call the function with the substring starting from the next character. If the characters are different, we move to the next character without any deletions.
