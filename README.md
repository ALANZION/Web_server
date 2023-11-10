# Developing a Simple Webserver
## NAME: ALAN ZION H
## REFERENCE NO:23013715
# AIM:

Develop a webserver to display about top five web application development frameworks.

# DESIGN STEPS:

## Step 1:

HTML content creation is done

## Step 2:

Design of webserver workflow

## Step 3:

Implementation using Python code
from http.server import HTTPServer, BaseHTTPRequestHandler
content ="""
<html>
<head>
</head>
<body>
<h1>ALAN ZION H</h1>
<h1>AIML</h1>
</body>
</html>
"""

class HelloHandler (BaseHTTPRequestHandler):
   def do_GET (self):
     self.send_response(200)
     self.send_header('Content-type', 'text/html; charset=utf-8')
     self.end.headers ()
     self.wfile.write(content.encode())

server_address = ('', 80)
httpd = HTTPServer (server_address, HelloHandler)
httpd.serve_forever()

## Step 4:

Serving the HTML pages.

## Step 5:

Testing the webserver
# PROGRAM:
```python   

from http.server import HTTPServer, BaseHTTPRequestHandler
content ="""
<html>
<head>
</head>
<body>
<h1>ALAN ZION H V</h1>
<h1>AIML<h1>
</body>
</html>
"""

class HelloHandler (BaseHTTPRequestHandler):
   def do_GET (self):
     self.send_response(200)
     self.send_header('Content-type', 'text/html; charset=utf-8')
     self.end.headers ()
     self.wfile.write(content.encode())

server_address = ('', 80)
httpd = HTTPServer (server_address, HelloHandler)
httpd.serve_forever()

```
# OUTPUT:
![webserver1](https://github.com/ALANZION/Web_server/assets/145743064/22984d20-d3b8-4b03-8339-a181c94eef83)


# RESULT:

The program is executed succesfully
