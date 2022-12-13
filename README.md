# Nested-Recursive-Loops-Using-Functions (Python)
I am having issues with this code that uses nested recursive loops

# Nested recursive loops

nested_recursive_loop_variable1 = 0


def nested_recursive_loop1(nested_recursive_loop_variable1):
    nested_recursive_loop_variable2 = 0
    if nested_recursive_loop_variable1 <= 2:
        print()
        print('Outer Recursive Loop')
        print('The value of the nested recursive loop variable 1 is', nested_recursive_loop_variable1)
        print('The value of the nested recursive loop variable 2 is', nested_recursive_loop_variable2)
        nested_recursive_loop_variable1 += 1
        nested_recursive_loop2(nested_recursive_loop_variable1, nested_recursive_loop_variable2)


def nested_recursive_loop2(nested_recursive_loop_variable1, nested_recursive_loop_variable2):
    if nested_recursive_loop_variable2 <= 2:
        print('Inner Recursive Loop')
        print('The value of the nested recursive loop variable 1 is', nested_recursive_loop_variable1)
        print('The value of the nested recursive loop variable 2 is', nested_recursive_loop_variable2)
        nested_recursive_loop_variable2 += 1
        nested_recursive_loop2(nested_recursive_loop_variable1, nested_recursive_loop_variable2)
    nested_recursive_loop1(nested_recursive_loop_variable1)


nested_recursive_loop1(nested_recursive_loop_variable1)
print()
