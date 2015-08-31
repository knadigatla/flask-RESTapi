# flask-RESTapi
Simple REST enabled webserver using python flask

use virtualenv(used virtualenverapper) - todo-flask

workon todo-flask

# run the app.py
(todo-flask)<hostname>:todo-flask <username>$ ./app.py
 * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
 * Restarting with stat

# sample curl commands
GET
curl -i http://127.0.0.1:5000/todo/api/v1.0/tasks
GET with options
curl -i http://127.0.0.1:5000/todo/api/v1.0/tasks/2
POST
curl -i -H "Content-Type: application/json" -X POST -d '{"title":"Read a book"}' http://localhost:5000/todo/api/v1.0/tasks
PUT
curl -i -H "Content-Type: application/json" -X PUT -d '{"done":true}' http://localhost:5000/todo/api/v1.0/tasks/2
