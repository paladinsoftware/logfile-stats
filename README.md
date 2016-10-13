# Logfile report
Simple command line report based on logfile from one day.

## Usage
Just use it like:
***REMOVED***
./report date
***REMOVED***
Where date is day from which you want to generate report in YYYY-MM-DD format.
For example:
***REMOVED***
./report 2016-10-10
***REMOVED***

## How it works
When running script for the first time with day it'll download log archive from
Papertrail service and unzip it to `./log_files` directory. Directory is
gitignored so don't worry about accidentally adding log file to git repo. After
getting file there's simple report generated with awk.

## Known issues
- newrelic (and probably honeybadger) performs `HEAD /` requests to check if
  site is up. This affects number of requests with `status=200` and `path="/"`.
  It would be probably best to just filter those requests out from stats.
- some requests are marked as failed by heroku (those with `code=XX`) and are
  filtered out right now. It's `~3000-4000` requests per day.
- requests with space in value of one of the parameters are filtered out. It's
  `~200` requests per day.

***REMOVED******REMOVED***:
***REMOVED***
***REMOVED***

***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***

***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***

***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***

***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***

***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
***REMOVED***
