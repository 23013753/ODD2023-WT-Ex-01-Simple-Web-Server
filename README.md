# Ex-01-Simple-Web-Server
Name : VISHAL.S REFERENCE NUMBER: 23013753 DEPARTMENT: AIML

## AIM:
To develop a simple webserver to serve html pages.

## DESIGN STEPS:
### Step 1: 
HTML content creation.

### Step 2:
Design of webserver workflow.

### Step 3:
Implementation using Python code.

### Step 4:
Serving the HTML pages.

### Step 5:
Testing the webserver.

## PROGRAM:
from http.server import HTTPServer, BaseHTTPRequestHandler

 content ="""

     <html>

       <head>

       </head>

       <body>

            <h1>Welcome</h1>

       </body>

     </html>
    class HelloHandler(BaseHTTPRequestHandler):
 
    def do_ GET(self):
        self.send_response(200)
        self.send_header('Content-type', 'text/html;charset=utf-8')
        self.end_headers()
        self.wfile.write(content.encode())




server address = ('', 80) 

httpd = HTTPServer (server_address, HelloHandler)

httpd.serve_forever()

## OUTPUT:
![image](https://github.com/23013753/ODD2023-WT-Ex-01-Simple-Web-Server/assets/145634121/4a1b0c6b-5e55-4f17-831a-c9a2212f8280)



## RESULT:
The program for implementing simple webserver is executed successfully.
