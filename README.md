# CAPTCHA Solver Application

This is a simple, single-page web application designed to demonstrate a basic client-side CAPTCHA solver. It features a responsive layout powered by Tailwind CSS and includes a mechanism to display a CAPTCHA image and allow users to submit their solution.

## Features

- **Dynamic CAPTCHA Image Loading**: Displays a CAPTCHA image, defaulting to `sample.png` or loading from a `url` query parameter (e.g., `?url=https://example.com/image.png`).
- **User Input**: An input field for users to type their CAPTCHA solution.
- **Client-Side Validation**: Compares the user's input against a hardcoded correct answer (based on the provided `ADCRB` image).
- **Responsive Design**: Adapts to various screen sizes using Tailwind CSS.
- **Clear Feedback**: Provides visual feedback on whether the CAPTCHA was solved correctly or not.
- **Reload Functionality**: Allows users to reload the current CAPTCHA or display the default if a URL was used.

## Getting Started

To get a copy of this project up and running on your local machine, follow these simple steps.

### Prerequisites

YouJust need a modern web browser to open the `index.html` file.

### Installation

1.  **Save the files**: Ensure `index.html`, `README.md`, `LICENSE`, and `sample.png` are all in the same directory.

2.  **Open in browser**: Simply open the `index.html` file with your preferred web browser.

## Usage

Upon opening `index.html`:

1.  **View CAPTCHA**: An image will be displayed (either `sample.png` or one specified by the `url` query parameter).
2.  **Enter Solution**: Type the text you see in the CAPTCHA image into the input field.
    *   *Hint*: For the default `sample.png`, the correct answer is `ADCRB` (case-insensitive).
3.  **Submit**: Click the "Submit" button to check your answer.
4.  **Reload**: Click the "Reload CAPTCHA" button to clear the input and message, and re-display the CAPTCHA image.

### Custom CAPTCHA Images

You can test with different images by passing a `url` query parameter in the browser's address bar. For example:

`file:///path/to/your/folder/index.html?url=https://example.com/another_captcha.png`

*Note: The client-side solver is hardcoded for 'ADCRB'. If you use a different image, you would need to modify the `correctCaptcha` variable in `index.html`'s JavaScript for the solver to work for that specific image.*