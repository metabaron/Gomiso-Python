Gomiso Python
=============

Python library for interacting with [Gomiso](http://www.gomiso.com/)

Purpose
-------
This library is my first attempt at coding using [Python](http://www.python.org/).
I learned Python while coding it so this is not the proper Python code you'll ever see but it's functional

Contributing
------------
When to contribut? Please contact [me](https://github.com/metabaron) instead of forking the project.

Usage
-----
The code is documented but here is a simple example of how to use the library:

	consumer_key = 'XXXXXX'
	consumer_secret = 'YYYYYY'
	username = 'AAAAA'
	password = 'BBBBB'
	tokensFile = 'path_to_file_where_we_will_store_tokens'
	
	letsGo = gomiso()
	if letsGo.authentification(consumer_key, consumer_secret, username, password, tokensFile):
		json_result = json.loads(letsGo.getUserInfo())
		print 'Hello user: ' + json_result['user']['username']
	else:
		print 'Something is wrong'

Documentation generated using the following command line:
	>python.exe pydoc.py -w gomiso
	wrote gomiso.html
	>
	
About me
-------------
You will find more about me through my [blog](http://blog.metabaron.net)