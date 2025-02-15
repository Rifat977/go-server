# Go Web Server Practice



This project is a simple Go web server built for practicing and learning the fundamentals of web development with Go. It demonstrates key concepts such as:



* **HTTP Handlers:** Creating and registering HTTP handlers to respond to different routes and methods.

* **Form Handling:** Parsing form data from POST requests.

* **Static File Serving:** Serving static files (e.g., HTML, CSS) from a directory.

* **Error Handling:** Implementing basic error handling for routes and methods.

* **Basic Routing:** Setting up simple route matching.

* **Dockerization:** Containerizing the application for easy deployment and portability.

* **Live Reloading:** Using `air` for live reloading during development.

* **Go Modules:** Managing project dependencies using Go modules.

* **Cross Compilation:** Building a linux executable from any OS.



## What I Practiced and Learned



* **Building a basic web server in Go:** I learned how to use the `net/http` package to create HTTP servers and handle requests.

* **Handling form data:** I practiced parsing form data from POST requests using `r.ParseForm()` and `r.FormValue()`.

* **Serving static files:** I learned how to serve static files from a directory using `http.FileServer()`.

* **Creating custom HTTP handlers:** I practiced creating custom HTTP handlers to handle specific routes and methods.

* **Implementing basic error handling:** I learned how to handle errors such as 404 not found and method not supported.

* **Dockerizing a Go application:** I learned how to create a Dockerfile to containerize my Go application.

* **Using Go modules:** I practiced managing project dependencies using Go modules.

* **Live Reloading with Air:** I implemented air to make development faster.

* **Cross Compilation:** I built a linux executable from my local machine.

## How to Run

### Locally

1.  **Clone the repository:**

    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2.  **Run the application:**

    ```bash
    go run main.go
    ```

3.  **Open your browser:**

    * Navigate to `http://127.0.0.1:8000` to access the static files.
    * Navigate to `http://127.0.0.1:8000/hello` to access the hello handler.
    * Navigate to `http://127.0.0.1:8000/form` and send post requests to test the form handler.

### With Docker

1.  **Clone the repository:**

    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2.  **Build the Docker image:**

    ```bash
    docker build -t go-server:latest .
    ```

3.  **Run the Docker container:**

    ```bash
    docker run -p 8000:8000 go-server:latest
    ```

4.  **Open your browser:**

    * Navigate to `http://localhost:8000` to access the application.

### With Air

1.  **Install Air:**

    ```bash
    go install [github.com/cosmtrek/air@latest](https://www.google.com/search?q=https://github.com/cosmtrek/air%40latest)
    ```

2.  **Clone the repository:**

    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

3.  **Run the application:**

    ```bash
    air
    ```

4.  **Open your browser:**

    * Navigate to `http://127.0.0.1:8000` to access the application.
