1. Install forever
# https://www.npmjs.com/package/forever
[sudo] npm install forever -g

[sudo] npm install -g http-server

forever start -c http-server ./app -a localhost -p 8000 -c-1

-c  COMMAND      COMMAND to execute (defaults to node)

http-server:
http-server [path] [options]
[path] defaults to ./public if the folder exists, and ./ otherwise.

-p Port to use (defaults to 8080)
-a Address to use (defaults to 0.0.0.0)
-c Set cache time (in seconds) for cache-control max-age header, e.g. -c10 for 10 seconds (defaults to '3600'). To disable caching, use -c-1.

openssl req -newkey rsa:2048 -new -nodes -x509 -days 3650 -keyout key.pem -out cert.pem
