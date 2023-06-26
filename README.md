# IPv4-IPv6-String-Check
The code checks whether a string is IPv4, IPv6, or Invalid

#IPv4 <br>
| Approach: The given problem can be solved by splitting the string with respect to ‘.’ while checking for IPv4 address and ‘:’ while checking for IPv6 address and check for the conditions for the string as IPv4 or IPv6 or Invalid.

Follow the steps below to check if the string is IPv4:

    1. Initialize a boolean variable, ans as true to check if the string is IPv4 or not.
    2. Store the count of occurrence of ‘.’ in the given string, S in a variable cnt.
    3. If the value of cnt is not equal to 3, then update the value of ans to false. Otherwise, tokenize the string, S with respect to the character ‘.’ and store the tokenized strings in an array V.
    4. Check if the size of V is equal to 4 or not. If not equal, update the value of ans to false.
    5. Otherwise, traverse the array, V and for each string, str in V check it lies in the range [0, 255] and does not contain leading 0s. If not, then update the value of ans to false.
    6. If the value of ans is true, then the string is a valid IPv4 address, Otherwise, it is not a valid IPv4 address.
