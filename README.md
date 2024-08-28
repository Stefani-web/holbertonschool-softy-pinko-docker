# Docker Project

This project aims to familiarize yourself with Docker by creating, configuring, and manipulating Docker containers to deploy a web application including a static front-end and a dynamic back-end API. The project is carried out in several stages, each adding additional features to the basic infrastructure.

## Project Goals
**Create a base Docker image:**

Using Ubuntu as the base image.\
Update packages with apt-get update.\
Upgrade installed packages with apt-get upgrade -y.\
The image should display "Hello, World!" when executed.\
Add a back-end with Flask:

Install Python3, pip3, and Flask.\
Create a Python api.py file using Flask to serve a simple route /api/hello returning **"Hello, World!"**\
Host the Flask application on port 5252.\
Develop a static front-end:

Create a front-end in HTML/CSS.
[Clone an existing front-end repository](https://github.com/atlas-school/softy-pinko-front-end) to integrate the UI.

Host static content with Nginx.
Connect the front-end and back-end:

Modify the front-end to dynamically retrieve data from the back-end API.
Use CORS to allow cross-origin requests.
Integrate JavaScript to interact with the API.
Set up a proxy server with Nginx:

Create a proxy server that acts as an intermediary between the client, the front-end, and the back-end.
Simplify interactions between the different parts of the application.
Centralize access via a single entry point (the proxy).
Add additional API servers and load balance:

Configure multiple instances of the API server to handle a larger volume of requests.
Using Nginx as a load balancer to distribute requests equally between different backend instances.

## Project Structure
**task0/ :** Create the base Docker image.\
**task1/ :** Add Python, pip and Flask for the backend.\
**task2/ :** Develop and integrate the static frontend.\
**task3/ :** Connect the frontend and backend, add dynamics via API.\
**task4/ :** Set up the Nginx proxy server.\
**task5/ :** Add additional API servers and load balance.\

## Execution
To run the project, use Docker and Docker Compose. For example, to start all services with load balancing, you can use:

bash
Copy Code

```
docker-compose up --scale back-end=2
```
This command will launch two instances of the API server, a frontend and a proxy server. You can access the application via http://localhost.

## Conclusion
This project demonstrates how to use Docker to deploy a complex web application with a static front-end, a dynamic back-end, and a load balancer to handle scaling. With Docker, it is possible to easily manage deployments, updates, and infrastructure in a repeatable way.

## License
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE X CONSORTIUM BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Except as contained in this notice, the name of <Stephanie CARVALHO> shall not be used in advertising or otherwise to promote the sale, use or other dealings in this Software without prior written authorization from <Stephanie CARVALHO>.

Copyright (c) 2024 [Stephanie Carvalho](https://github.com/Stefani-web)

## Author
[Stephanie Carvalho](https://github.com/Stefani-web)
