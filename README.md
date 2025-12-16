# dataurl
parsing and generation of data: urls in python

Yes, since py3.4 we have [urllib.request.DataHandler](https://docs.python.org/3/library/urllib.request.html#datahandler-objects),
which is probably preferable for "I found a data: thing and want to get what's in there" needs.

This is meant as a fallback, and some exploration of what can be in there.
