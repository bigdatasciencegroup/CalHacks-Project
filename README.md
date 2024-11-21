# Project Montgomery

Built by Team Recursive Bruins
- Jonathan Ouyang
- Johnny Zheng
- Justin Osbey
- Eric Zhou

## Project overview

Project Montgomery is a tool designed to assist users in visual learning, particularly in mathematics, physics, and computer science. It leverages the power of visual animations using the Manim library and integrates with Google's Gemini API for generating responses and animations based on user input.

## Features

* Text-to-speech feedback
* Manim-based animations
* Integration with Google's Gemini API
* FastAPI backend for handling user requests

## Installation

1. Clone the GitHub repository:
    ```bash
    git clone https://github.com/JonOuyang/CalHacks-Project
    ```

2. Create the environment for the project using the command:
    ```bash
    conda env create -f environment.yml
    ```

3. Install required modules for Google Gemini API:
    ```bash
    pip install -q -U google-generativeai
    ```

4. Install required modules for the rest of the project:
    ```bash
    pip install -r fastapi/requirements.txt
    ```

## Usage

1. Activate the conda environment:
    ```bash
    conda activate calhacks
    ```

2. Run the FastAPI server:
    ```bash
    uvicorn fastapi/api/main2:app --reload
    ```

3. Access the application at `http://localhost:8000`.

## Project structure

* `environment.yml`: Contains the conda environment configuration.
* `fastapi/api/external_functions.py`: Contains functions for text-to-speech and Manim animations.
* `fastapi/api/gemini_call.py`: Handles calls to the Google Gemini API.
* `fastapi/api/main2.py`: Main FastAPI application file.
* `fastapi/api/manim_script.py`: Example Manim script.
* `fastapi/requirements.txt`: Contains the Python dependencies for the FastAPI application.
* `frames.py`: Script to split an MP4 video into frames.
* `playground.py`: Script for testing and executing code.
* `scraper.py`: Script to scrape the Manim reference manual.

## Contributing

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -am 'Add new feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Create a new Pull Request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
