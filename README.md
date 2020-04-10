#Dir Watcher
Creates a long running program named `dirwatcher.py`.  This program continuously searches all files within a given directory for a 'magic' string that is passed as a command line argument.  

Once the 'magic' string is located, a message is logged indicating that it has been found, the file that it was found in, as well as the corresponding line number.

This program will terminate itself 
by catching SIGTERM or SIGINT.

usage: dirwatcher.py [-h] [-e EXT] [-i INTERVAL] path magic

positional arguments:
  path                  Directory path to watch
  magic                 String to watch for

optional arguments:
  -h, --help            show this help message and exit
  -e EXT, --ext EXT     Text file extension to watch
  -i INTERVAL, --interval INTERVAL
                        Number of seconds between polling