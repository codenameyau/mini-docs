mini-docs
=========

###Minimal Docstrings Convention

- [Python Example](#python-example)
- [Ruby Example](#ruby-example)
- [C Example](#c-example)
- [Scheme Example](#scheme-example)
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

        ! Use add_two_numbers() instead.

        Adds the two numbers.
        """
        pass

```

##Ruby Example
```ruby

    # Public: sum(Integer, Integer) -> Integer
    # Returns the sum of first and second
    #
    # Example:
    # >> sum(10, 30)
    # => 40
    def sum(a, b)
        return first + second
    end

```

##C Example
```c

    // Public: sum(int first, int first) -> int
    // Computes the sum of first and second
    //
    // Example:
    // sum(2, 4) => 6
    int sum(int first, int second) {
        return(first + second);
    }

```

##Scheme Example
```scheme

    ;; Public: (Integer Integer) -> Integer
    ;; Returns the sum of first and second
    ;;
    ;; Example:
    ;; > (sum-numbers 4 5)
    ;; 9
    (define (sum-numbers first second)
      (+ first second))

```

##General Guidelines

```

    def descriptive_name(argument_1, argument_2):
        """
        FUNCTION_USAGE: (type of argument_1, ...) -> return type

        FUNCTION_DESCRIPTION

        EXAMPLE:
        """
        ...

```

1. Each of the examples above have slight variations, but the overall goal is to clearly and succinctly describe the function's usage in a human readable format.

2. For the function name and arguments, spell out words or use acronyms.
    - For the function name, consider starting with a verb (ex. `add_numbers`, `send_request`)

3. FUNCTION_USAGE:
    - Choose: Public, Internal, Private, DEPRECATED

4. FUNCTION_DESCRIPTION:
    - Briefly describe what the function accomplishes. If your description is too long, consider splitting the function into smaller functions.

5. EXAMPLE:
    - Include an example if the FUNCTION_USAGE is Public. Otherwise examples are optional.

