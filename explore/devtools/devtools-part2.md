1. Even though num1 and num2 may look like numbers, their values come from .value on input fields, which always return strings. So "2" + "3" results in "23", not 5. That’s string concatenation, not addition.
2. I would fix it by first converting num1 and num2 to integers and then adding them.
