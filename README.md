# Simple Go Web Server

A basic web server built with Go that handles form submissions, serves static files, and supports basic routing and error handling.

## Features

- Handles form submissions via POST requests.
- Serves static files from the `./static` directory.
- Supports simple GET requests with a custom handler (`/hello`).
- Returns appropriate error messages for unsupported methods or paths.

## Installation

1. Clone this repository or download the source code.

    ```bash
    git clone https://github.com/your-username/simple-go-web-server.git
    ```

2. Make sure you have [Go](https://golang.org/doc/install) installed.

3. Navigate to the project directory and install any dependencies (if applicable).

    ```bash
    cd simple-go-web-server
    ```

## Usage

1. Create a `static` directory in the project root and add any static files (HTML, CSS, JS) you want to serve.

2. Run the Go server:

    ```bash
    go run main.go
    ```

3. The server will be available at `http://localhost:8080`.

4. Test the following endpoints:
   - `GET /hello` - Returns "hello!"
   - `POST /form` - Handles form submissions (requires `name` and `address` fields).

## Example Form

```html
<form action="/form" method="POST">
    <input type="text" name="name" placeholder="Enter your name">
    <input type="text" name="address" placeholder="Enter your address">
    <button type="submit">Submit</button>
</form>
```
