# CS510 Project 3: MicroML-to-AST Translator
  by Bowen Madden, Combee-3

This project is a web-based application for parsing and visualizing Abstract Syntax Trees (AST) for the MicroML language described in the class textbook & homeworks. It allows users to input MicroML code, parse it into an AST, and display the tree structure visually on a web page.

## Features

- **MicroML Parsing**: Parses MicroML code into an Abstract Syntax Tree (AST) using a custom lexer and parser.
- **AST Visualization**: Displays the AST as an interactive tree diagram on the web page.
- **Dynamic Input**: Users can input MicroML code directly into the web app and see the resulting AST in real-time.
- **Web-Based**: Built using ASP.NET Core and Giraffe for the backend, with a JavaScript-based frontend for rendering the AST.
- **Customizable Styling**: Includes CSS for styling the web page and options for customizing the tree visualization.

## Requirements

- .NET 6.0 or later
- A modern web browser (for the frontend)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Combee-3/project-3-CS510-combee-3.git
   cd project-3-CS510-combee-3

2. Build the project with:
    dotnet build

3. Run the application with:
    dotnet run

4. Open your web browser and navigate to the URL specified in the terminal, or follow the link directly from the terminal.

## Usage

1. Enter MicroML code in the input box on the web page.

2. Click the "Parse and Draw AST button to generate your AST

3. View the AST. You can download it as an image file as well.
    Example MicroML code: let x = 5 in x + 10

## Project Structure:

- Fun.fs: Contains the core evaluation logic for MicroML expressions.
- Parse.fs: Implements the parser for MicroML code using FunLex and FunPar.
- Program.fs: Configures the ASP.NET Core web server and routes.
- View/index.html: The main HTML file for the web app. Stylized by wwwroot/default.css
- wwwroot/: Contains the JavaScript, CSS, and other static assets for the web page frontend.

## Technologies Used:

- Backend: F#, ASP.NET Core, & Giraffe
- Frontend: JavaScript, HTML, & CSS as mentioned above.
- Parsing: FsLex and FsYacc, for both lexical analysis and parsing.

## License:
This project uses the MIT license. See LICENSE.txt for details.

## Acknowledgements & Credit:
- The jsSyntaxTree library is used for rendering syntax trees in the frontend.
- Special thanks to the creators of FsLex and FsYacc for enabling the parsing functionality.
- I started with a code base written by my professor in-class, and after analyzing it, made edits of my own to fulfill the remaining requirements. This is a class project for learning purposes and personal experience.