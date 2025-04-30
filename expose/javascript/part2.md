1. line 12 will print 3. In JavaScript, var has function scope, not block scope. That means i is accessible anywhere inside the function discountPrices, including after the for loop, such as in line 12.
2. line 13 will print 150. discountedPrice is declared using var, which has function scope (not block scope). So even though it is declared inside the for loop block, it is accessible throughout the discountPrices function.
3. line 14 will print 150. During each iteration of the loop, finalPrice is updated with the discounted price of the current element in the prices array. After the loop ends, finalPrice will hold the value of the last discounted price in the array. So, at line 14, finalPrice will be printed with the discounted price of the last item in prices.
4. nothing will be printed to the console after the function call because the only output inside the function is the console.log(finalPrice) statement, which will no longer execute.
5. ReferenceError: i is not defined. This is because i is only defined within the scope of the for loop. Unlike var, let is block-scoped so the program does not know what i is.
6. ReferenceError: discountedPrice is not defined. Like the previous example, discountedPrice is also only declared within a block-scope using let.
7. 150. finalPrice is initialized in the global scope so can be accessed after the for loop as well.
8. [ 50, 100, 150 ] because after the loop ends, the discounted array contains all the discounted prices. The function then returns the discounted array.
9. ReferenceError: i is not defined. Using const inside the for loop gives i block scope, making it inaccessible outside the loop. Attempting to log i after the loop results in a ReferenceError.
10. 3. discountedPrice is initialized outside the scope.
11. [ 50, 100, 150 ] The function calculates discounted prices by applying the discount to each item in the prices array. It stores each discounted price in the discounted array. It then returns the discounted array.
12. A. student.name
    B. student["Grad Year"]
    C. student.greeting()
    D. student["Favorite Teacher"].name
    E. student.courseLoad[0]
13. A. 32. + triggers string concatenation when one operand is a string.
    B. 1. - triggers numeric conversion; '3' becomes 3, then 3 - 2 = 1.
    C. 3. null converts to 0, so 3 + 0 = 3
    D. 3null. null becomes 'null', then concatenated as a string.
    E. 4. true converts to 1, so 1 + 3 = 4.
    F. 0. false and null both convert to 0 so it is 0 + 0.
    G. 3undefined. undefined becomes 'undefined', then concatenated as a string.
    H. NaN. '3' becomes 3, but undefined cannot convert to a number, so the result is NaN.
14. A. true. '2' converts to 2, and 2 > 1 is true.
    B. false. Both are strings; compared lexicographically, '2' > '1', so result is false.
    C. true. == allows type coercion; '2' becomes 2.
    D. false. === checks both value and type; number !== string.
    E. false. true is 1, which is not equal to 2.
    F. true. Boolean(2) is true; types and values match, so true === true.
15. == checks for equality after type conversion (loose equality). === checks for equality without type conversion (strict equality), so both value and type must be the same.

17. [ 2, 4, 6 ]. modifyArray takes two arguments: an array and a callback function. It loops through the array [1, 2, 3]. For each element, it calls doSomething(num):When num = 1, returns 2. When num = 2, returns 4. When num = 3, returns 6. These results are pushed to a new array, which becomes [2, 4, 6].

19. 1
4
3
2
