1. The console will print prices.length, which in this case is 3, as that is the value of i at the end of the loop, and since i is defined with a var keyword, it's accessible outside of the for loop.
2. The console will print 150 as that is the last value of discountedPrice (300 * 0.5 = 150), and it's still accessible since it was declared with the var keyword.
3. The console will print 150 as that is the last value of finalPrice as well.
4. It will return the array [50, 100, 150]. In the for loop, the discounted price of each input price is calculated and pushed to the discounted array. At the end of the loop, the array is then returned.
5. An error would occur since i is limited in scope to the for loop, so it cannot be accessed outside of it, such as in line 12.
6. An error would occur as well since discountedPrice is declared within the for loop using a let keyword and is therefore limited in scope to the for loop. Since the console.log() in line 13 is outside the for loop, discountedPrice is not accessible there.
7. The console will print 150 as that is the last value of finalPrice. It is accessible on line 14 as finalPrice was declared on line 4, so its scope is that of the function body; as the console.log() in line 14 is within the function body, finalPrice is accessible there.
8. The function will return the same array as the previous function did; it shall return the array [50, 100, 150]. In the for loop, the discounted price of each price is computed and pushed into the discounted array. Since the discounted array is declared outside of the for loop, it is accessible in the rest of the function, and so can be returned on line 16 without errors.
9. The code will error out as i is limited in scope to the for loop, and so it cannot be accessed outside of it in line 11.
10. length is a constant that is defined once at the top of the function, so as it is never reassigned and is accessed on line 12 which is in the function, the console.log will print prices.length, which is 3 with the given input.
11. This code will return the same array as before, as pushing to an array does not count as reassigning it to another value, so line 8 will not cause an error. The array returned will be [50, 100, 150] since the discounted array consists of the discounted prices of each price in the prices input array.
12. A. student.name
    B. student['Grad Year']
    C. student.greeting()
    D. student['Favorite Teacher'].name
    E. student.courseLoad[0]
13. A. '3' + 2 evaluates to '32' since the '2' is converted to a string and the addition performs string
    concatenation.
    B. '3' - 2 evaluates to 1 since the '3' is converted to a number and subtraction is performed to calculate 3 - 2 = 1.
    C. 3 + null evaluates to 3 since null is converted to 0 and 3 + 0 = 3.
    D. '3' + null evaluates to '3null' since null is converted to the string 'null' and the addition performs string concatenation.
    E. true + 3 evaluates to 4 since true is converted to 1 and 1 + 3 = 4.
    F. false + null evaluates to 0 since false is converted to 0, null is converted to 0, and 0 + 0 = 0.
    G. '3' + undefined evaluates to '3undefined' since undefined is converted to the string 'undefined' and the addition performs string concatenation.
    H. '3' - undefined evaluates to NaN since undefined is converted to NaN and 3 - NaN is NaN.
14. A. '2' > 1 evaluates to true since '2' is converted to the number 2 and 2 > 1 is true.
    B. '2' < '12' evaluates to false since the strings are compared in lexicographical order, and '2' comes after '1' in this order.
    C. 2 == '2' evaluates to true as '2' is converted to the number 2, which equals itself.
    D. 2 === '2' evaluates to false as these two values are of different types and require a type conversion to equal one another.
    E. true == 2 evaluates to false since true is converted to the number 1, and 1 != 2.
    F. true === Boolean(2) evaluates to true since Boolean(2) evaluates to true, and true equals itself without type conversion.
15. The == operator checks equality of two different values after converting both values to the same type; hence, 2 == '2' is true since '2' is converted to the number 2. The === operator does not convert the values' types, and so in order for a === b to be true, it must be the case that a == b and that a and b are of the same type.
17. First, we call `modifyArray([1,2,3], doSomething);` which passes the array `[1,2,3]` and the callback function `doSomething` to `modifyArray`. We create `newArr`, and for every element in `[1,2,3]`, we push the result of `doSomething(array[i])`. Since `doSomething(n)` returns `2 * n`, we'll push `2`, `4`, and `6` into `newArr` in that order. Since we return `newArr`, the result of this operation is `[2,4,6]`.
19. The output will be 1 4 3 2.