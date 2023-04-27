1. values added: 20
2. final result: 20
3. values added: 20
4. Error, since result cannot be identified (the scope of the result variable is within the if's then block, and so is not accessible outside of the if statement).
5. Error occurs in line 7 because you can't reassign a value to a const variable.
6. Error occurs in line 13 since the scope of the const variable limits it to the if's then block, so it's not accessible outside of the if (this error would be caught only if line 7 is fixed, otherwise JavaScript wouldn't try to run that line).