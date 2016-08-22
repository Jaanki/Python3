Integers
----------
>>> a = 1
>>> a 
  1
>>> type(a)
  <class 'int'>
>>> dir(a)
  ['__abs__', '__add__', '__and__', '__bool__', '__ceil__', '__class__', '__delattr__', '__dir__', '__divmod__', '__doc__', '__eq__', '__float__', '__floor__', '__floordiv__', '__format__', '__ge__', '__getattribute__', '__getnewargs__', '__gt__', '__hash__', '__index__', '__init__', '__int__', '__invert__', '__le__', '__lshift__', '__lt__', '__mod__', '__mul__', '__ne__', '__neg__', '__new__', '__or__', '__pos__', '__pow__', '__radd__', '__rand__', '__rdivmod__', '__reduce__', '__reduce_ex__', '__repr__', '__rfloordiv__', '__rlshift__', '__rmod__', '__rmul__', '__ror__', '__round__', '__rpow__', '__rrshift__', '__rshift__', '__rsub__', '__rtruediv__', '__rxor__', '__setattr__', '__sizeof__', '__str__', '__sub__', '__subclasshook__', '__truediv__', '__trunc__', '__xor__',  'bit_length','conjugate', 'denominator', 'from_bytes', 'imag', 'numerator', 'real', 'to_bytes']
>>> help(a.bit_length)
  Help on built-in function bit_length:
  bit_length(...) method of builtins.int instance
      int.bit_length() -> int
      
      Number of bits necessary to represent self in binary.
      >>> bin(37)
      '0b100101'
      >>> (37).bit_length()
      6
>>> float(a)
  1.0
>>> str(a)
  '1'
>>> del(a)
>>> a
  Traceback (most recent call last):
    File "<stdin>", line 1, in <module>
  NameError: name 'a' is not defined

Float
------
>>> a = 1.0
>>> type(a)
  <class 'float'>
>>> dir(a)
  ['__abs__', '__add__', '__bool__', '__class__', '__delattr__', '__dir__', '__divmod__', '__doc__', '__eq__', '__float__', '__floordiv__', '__format__', '__ge__', '__getattribute__', '__getformat__', '__getnewargs__', '__gt__', '__hash__', '__init__', '__int__', '__le__', '__lt__', '__mod__', '__mul__', '__ne__', '__neg__', '__new__', '__pos__', '__pow__', '__radd__', '__rdivmod__', '__reduce__', '__reduce_ex__', '__repr__', '__rfloordiv__', '__rmod__', '__rmul__', '__round__', '__rpow__', '__rsub__', '__rtruediv__', '__setattr__', '__setformat__', '__sizeof__', '__str__', '__sub__', '__subclasshook__', '__truediv__', '__trunc__', 'as_integer_ratio', 'conjugate', 'fromhex', 'hex', 'imag', 'is_integer', 'real']
>>> int(a)
  1
>>> str(a)
  '1.0'

String
-------
>>> string1 = "hi, This is python3 workshop"
>>> string1
  'hi, This is python3 workshop'
>>> dir(string1)
  ['__add__', '__class__', '__contains__', '__delattr__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__', '__getattribute__', '__getitem__', '__getnewargs__', '__gt__', '__hash__', '__init__', '__iter__', '__le__', '__len__', '__lt__', '__mod__', '__mul__', '__ne__', '__new__', '__reduce__', '__reduce_ex__', '__repr__', '__rmod__', '__rmul__', '__setattr__', '__sizeof__', '__str__', '__subclasshook__', 'capitalize', 'casefold', 'center', 'count', 'encode', 'endswith', 'expandtabs', 'find', 'format', 'format_map', 'index', 'isalnum', 'isalpha', 'isdecimal', 'isdigit', 'isidentifier', 'islower', 'isnumeric', 'isprintable', 'isspace', 'istitle', 'isupper', 'join', 'ljust', 'lower', 'lstrip', 'maketrans', 'partition', 'replace', 'rfind', 'rindex', 'rjust', 'rpartition', 'rsplit', 'rstrip', 'split', 'splitlines', 'startswith', 'strip', 'swapcase', 'title', 'translate', 'upper', 'zfill']
>>> string1.capitalize()
  'Hi, this is python3 workshop' - Only the first character got captitalised. Rest all in lower case


Concatinate:
>>> string1 + string2
  'Hi, this is string1string2' -- Notice no space

Multiply:
>>> string2 * 2
  'string2string2'

Lists
------
>>> list1 = ['a', 'b']
>>> list1
  ['a', 'b']
>>> type(list1)
  <class 'list'>
>>> dir(list1)
  ['__add__', '__class__', '__contains__', '__delattr__', '__delitem__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__', '__getattribute__', '__getitem__', '__gt__', '__hash__', '__iadd__', '__imul__', '__init__', '__iter__', '__le__', '__len__', '__lt__', '__mul__', '__ne__', '__new__', '__reduce__', '__reduce_ex__', '__repr__', '__reversed__', '__rmul__', '__setattr__', '__setitem__', '__sizeof__', '__str__', '__subclasshook__', 'append', 'clear', 'copy', 'count', 'extend', 'index', 'insert', 'pop', 'remove', 'reverse', 'sort']

>>> list1.append('c')
>>> list1
  ['a', 'b', 'c']
>>> list1.append(1)
>>> list1
  ['a', 'b', 'c', 1]

>>> list1.count(a)
  1
>>> list1.count(list1)
  0
>>> list1.count(1)
1
>>> list1.append('a')
>>> list1
  ['a', 'b', 'c', 1, 'a']
>>> list1.count('a')
  2
>>> list1.extend('q')
>>> list1
  ['a', 'b', 'c', 1, 'a', 'q']
>>> list1[0]
  'a'
>>> list1[-1]
  'q'
>>> list1[0:2]
  ['a', 'b']
>>> list1[-3:-1]
  [1, 'a']
>>> list1[:5]
  ['a', 'b', 'c', 'd', 1]
>>> list1[:50]
  ['a', 'b', 'c', 'd', 1, 'a', 'q']
>>> list1[2:]
  ['c', 'd', 1, 'a', 'q']
>>> list1.insert(3, 'd')
>>> list1
  ['a', 'b', 'c', 'd', 1, 'a', 'q']
>>> list1.index('b')
  1
>>> list1.index('a')
  0
>>> list1
  ['a', 'b', 'c', 'd', 1, 'a', 'q']
>>> list1.reverse()
>>> list1
  ['q', 'a', 1, 'd', 'c', 'b', 'a']
>>> list1.sort()
  Traceback (most recent call last):
    File "<stdin>", line 1, in <module>
  TypeError: unorderable types: int() < str()
>>> list1.remove('a')
>>> list1
  ['q', 1, 'd', 'c', 'b', 'a']
>>> list1.remove('1')
  Traceback (most recent call last):
    File "<stdin>", line 1, in <module>
  ValueError: list.remove(x): x not in list
>>> list1.remove(1)
>>> list1
  ['q', 'd', 'c', 'b', 'a']
>>> list1.sort()
>>> list1
  ['a', 'b', 'c', 'd', 'q']
>>> list1.pop('q')
  Traceback (most recent call last):
    File "<stdin>", line 1, in <module>
  TypeError: 'str' object cannot be interpreted as an integer
>>> list1.pop(3)
  'd'
>>> list1
  ['a', 'b', 'c', 'q']

tuples
-------
>>> tuple1 = ('a', 'b', 'c')
>>> tuple1
  ('a', 'b', 'c')
>>> type(tuple1)
  <class 'tuple'>
>>> dir(tuple1)
  ['__add__', '__class__', '__contains__', '__delattr__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__', '__getattribute__', '__getitem__', '__getnewargs__', '__gt__', '__hash__', '__init__', '__iter__', '__le__', '__len__', '__lt__', '__mul__', '__ne__', '__new__', '__reduce__', '__reduce_ex__', '__repr__', '__rmul__', '__setattr__', '__sizeof__', '__str__', '__subclasshook__', 'count', 'index']
>>> tuple1.count('a')
  1
>>> tuple1.index('b')
  1

Dictionary
------------
>>> dict1 = {'language': 'python', 'version': 3}
>>> dict1
  {'version': 3, 'language': 'python'}
>>> dict1['language']
  'python'
>>> dict1['version']
  3
>>> dir(dict1)
  ['__class__', '__contains__', '__delattr__', '__delitem__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__', '__getattribute__', '__getitem__', '__gt__', '__hash__', '__init__', '__iter__', '__le__', '__len__', '__lt__', '__ne__', '__new__', '__reduce__', '__reduce_ex__', '__repr__', '__setattr__', '__setitem__', '__sizeof__', '__str__', '__subclasshook__', 'clear', 'copy', 'fromkeys', 'get', 'items', 'keys', 'pop', 'popitem', 'setdefault', 'update', 'values']
>>> dict1.keys()
  dict_keys(['version', 'language'])
>>> dict1.values()
  dict_values([3, 'python'])
>>> dict1.items()
  dict_items([('version', 3), ('language', 'python')])
>>> dict1.get('language')
  'python'
>>> dict1.get('workshop', 101)
  101
>>> dict1
  {'version': 3, 'language': 'python'}
>>> dict1.pop('version')
  3
>>> dict1
  {'language': 'python'}
>>> dict1.popitem()
  ('language', 'python')
>>> dict1
  {}
>>> dict1['language'] = 'python'
>>> dict1
  {'language': 'python'}
>>> dict2 = dict1.copy()
>>> dict2
  {'language': 'python'}
>>> dict1
  {'language': 'python'}
>>> dict1.clear()
>>> dict1
  {}
