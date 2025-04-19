# python-not-operator

Checking the emptiness of a Python list is rather easy using the len() function. Yet, there's another technique that works on all types of sequences and collections. This is based on the truth value testing of the sequence or collection itself.

By default, a Python object is considered truthy unless its class defines either a **bool**() or a **len**() method that returns False or 0 respectively. Python's built-in objects, such as tuples, lists, strings, dictioners, sets and ranges all implement a **len**() method. This menas that truth value testing of these objects will return False if they are empty, and True otherwise.

Based on these observations, all you need to check if a Python list is empty is to test its truth value, using the not operator.

x = []
not x # True
y = [1, 2]
not y # False

that's it !!
