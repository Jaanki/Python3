Mutable - Can be changed
Immutable - Can't be changed

Integers
--------
>>> a = 1
>>> a
  1
>>> a = 2
>>> a
  2
  
Float
-----
>>> b = 1.0
>>> b
  1.0
>>> b = 2.0
>>> b
  2.0
  
String
------
>>> str1 = 'mutable or not'
>>> str1
  'mutable or not'
>>> str1[0] = 'im'
  Traceback (most recent call last):
    File "<stdin>", line 1, in <module>
  TypeError: 'str' object does not support item assignment
>>> str1 = 'immutable'
>>> str1
  'immutable'

List
----
>>> list1 = [1,2]
>>> list1
  [1, 2]
>>> list1[0] = 3
>>> list1
  [3, 2]
  
Tuple
-----
>>> tuple1 = (1,2)
>>> tuple1
  (1, 2)
>>> tuple1[0] = 3
  Traceback (most recent call last):
    File "<stdin>", line 1, in <module>
  TypeError: 'tuple' object does not support item assignment
>>> tuple1
  (1, 2)
  
Dictionary
----------
>>> dict1 = {'a':1, "b":2}
>>> dict1
  {'b': 2, 'a': 1}
>>> dict1[a] = 2
>>> dict1
  {'b': 2, 'a': 1, 2: 2} - can anybody explain what happened here
>>> dict1 = {'a':3, "b":2}
>>> dict1
  {'b': 2, 'a': 3}
