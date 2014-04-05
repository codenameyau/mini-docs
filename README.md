mini-docs
=========

###Minimal Docstrings

- [Python](#python-example)
- [JavaScript](#javascript-example)
- [General Guidelines](#general-guidelines)

##Python Example
```python

    def add_two_numbers(first, second):
        """
        Public: (Integer, Integer) -> Integer

        Returns the sum of first and second.

        Example:
        >>> add_two_numbers(2, 2)
        >>> 4
        """
        pass


    def is_number_in_list(target, numbers):
        """
        Internal: (Integer, List) -> Boolean

        Checks if the target integer is in numbers.
        """
        pass


    def _sort_numbers(numbers):
        """
        Private: (List) -> List

        Sorts and returns list of numbers
        """
        pass


    def deprecated_function(first, second):
        """
        DEPRECATED: (Integer, Integer) -> Integer

        ! Use is_number_in_list() instead.

        Adds the two numbers.
        """
        pass

```


##General Guidelines

```

    function descriptive_name(argument_1, argument_2)
        """
        FUNCTION_USAGE: (type of argument_1, ...) -> return type

        FUNCTION_DESCRIPTION

        EXAMPLE:
        """

```

1. For the function name and arguments, spell out words or use acronyms.

2. FUNCTION_USAGE:

    - Choose: Public, Internal, Private, DEPRECATED

3. FUNCTION_DESCRIPTION:

    - Give a brief description of what the function accomplishes. If you can't be brief, consider splitting the function into smaller functions.

4. EXAMPLE:

    - Mandatory for Public usuage. Otherwise example is optional.


