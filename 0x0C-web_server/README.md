# 0x0C-web_server

## Description

`0x0C-web_server` is a simple web server project designed to provide a basic understanding of how web servers work. The project focuses on creating a simple web server capable of handling HTTP requests and serving static web pages.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Contributing](#contributing)
- [License](#license)

## Installation

To install and run the web server, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/0x0C-web_server.git
   ```

2. Navigate to the project directory:

   ```bash
   cd 0x0C-web_server
   ```

3. Compile the source code:

   ```bash
   gcc -Wall -Werror -Wextra -pedantic *.c -o web_server
   ```

4. Run the web server:

   ```bash
   ./web_server
   ```

## Usage

Once the web server is running, it will listen for incoming HTTP requests on the specified port (default is port 8080). You can access the server by opening a web browser and navigating to `http://localhost:8080` or the specified port.

You can customize the port and other settings by modifying the configuration in the `config.h` file.

## Features

- **HTTP Server:** Provides a basic HTTP server capable of handling GET requests.
- **Static Content:** Serves static HTML and text files from the `www` directory.
- **Configurable:** Easily configurable through the `config.h` file.
- **Logging:** Logs incoming requests and server responses to the console.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/your-feature`.
3. Make your changes and commit them: `git commit -m 'Add some feature'`.
4. Push to the branch: `git push origin feature/your-feature`.
5. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
