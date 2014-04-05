mini-docs
=========

###Minimal Docstrings

```python

    def add_two_numbers(first, second):
        """
        Public: (Integer, Integer) -> Integer

        Returns the sum of the first and second.

        Example:
        >>> add_two_numbers(2, 2)
        >>> 4
        """
        pass


    def is_number_in_list(target, numbers):
        """
        Internal: (Integer, List) -> Boolean

        Checks if the target number is in the given
        list of numbers.
        """
        pass


    def _sort_numbers(numbers):
        """
        Private: (List) -> List

        Sorts and returns numbers
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
