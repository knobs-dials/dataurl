# dataurl
parsing and generation of data: urls in python - the things that look like `data:text/plain;base64,SGVsbG8sIFdvcmxkIQ==`

Yes, since py3.4 we have [urllib.request.DataHandler](https://docs.python.org/3/library/urllib.request.html#datahandler-objects),
which is probably preferable for "I found a data: thing and want to get what's in there" needs:
you hand the data url to urllib.request.urlopen() and get a response that you can `.read()` and get the `.headers` of.

This is meant 
- as a fallback
- as some exploration of what can be in there.
- as a generator, with a little control.

