Staircase Time Complexity: The time complexity of this code is O(n^2), where 'n' is the input or size of our staircase. 
The outer loop runs 'n' times, and for each iteration of the outer loop, the inner loops run a total of 'n' 
times. As a result, the overall time complexity is proportional to n * n, which simplifies to O(n^2).

Staircase Space Complexity: The space complexity of this code is O(1) or constant. The code does not make any extra calls that would impact 
the input. It is only used to determine the size of the stircase. Therefore, the space complexity is considered constant, O(1).

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
