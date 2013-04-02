curconv
=======

Curconv is a command-line currency conversion tool. It fetches exchange rates
from Google, and then caches them for 24 hours to improve response time.

Usage
-----

	# Convert $10 US dollars to Euros.
	$ curconv USD EUR 10
	USD 10.00 = EUR 7.64

	# Convert $1 Mexican peso to US dollars.
	$ curconv MXN USD
	MXN 1.0000 = USD 0.0782

	# Convert a million US dollars to Euros. (Note that commas are ignored.)
	$ curconv USD EUR 1,000,000
	USD 1000000.00 = EUR 771010.02

	# Convert ¥1000 Japanese yen to US dollars, bypassing the cache entirely.
	$ curconv --skip-cache JPY USD
	JPY 1.0000 = USD 0.0127
