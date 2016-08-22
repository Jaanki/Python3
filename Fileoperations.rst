Files
-----
>>> f = open('python3.txt')
>>> dir(f)
  ['_CHUNK_SIZE', '__class__', '__del__', '__delattr__', '__dict__', '__dir__', '__doc__', '__enter__', '__eq__', '__exit__', '__format__', '__ge__', '__getattribute__', '__getstate__', '__gt__', '__hash__', '__init__', '__iter__', '__le__', '__lt__', '__ne__', '__new__', '__next__', '__reduce__', '__reduce_ex__', '__repr__', '__setattr__', '__sizeof__', '__str__', '__subclasshook__', '_checkClosed', '_checkReadable', '_checkSeekable', '_checkWritable', '_finalizing', 'buffer', 'close', 'closed', 'detach', 'encoding', 'errors', 'fileno', 'flush', 'isatty', 'line_buffering', 'mode', 'name', 'newlines', 'read', 'readable', 'readline', 'readlines', 'seek', 'seekable', 'tell', 'truncate', 'writable', 'write', 'writelines']
>>> f.read()
  'Hi\nThis is a file.\nIt is for Python3 workshop.\n'
>>> f.read()
  ''
>>> f.write('hello')
  Traceback (most recent call last):
    File "<stdin>", line 1, in <module>
  io.UnsupportedOperation: not writable
>>> f.readable()
  True
>>> f.writable()
  False
>>> f.close()
  Check the file
>>> f = open('python3.txt', 'w')
>>> f.write('hi\nthis is python3')
  18
>>> f.close()
  Check the file
