# Moving and Coloring Square

This project implements a pure JavaScript function that creates a black square in the top-left corner of the browser window. After a 1 second pause, the square moves smoothly to the right while simultaneously sending a GET request to a specified URL. The square's color changes based on the server's response.

## Requirements

- The function should be executed in the latest version of Google Chrome.
- It should be called on an empty browser page (with an empty `<body>` tag).

## Function Behavior

1. **Initial Setup**:
    - A black square with a side length of 100 px is drawn at the top-left corner of the window when the function is invoked.

2. **Movement and Fetch**:
    - One second after being called, the square starts moving to the right at a constant speed of 100 pixels per second.
    - Simultaneously, a GET request is sent to the specified URL.

3. **Stopping the Square**:
    - After traveling a total distance of 100 pixels (1 second), the square stops moving.
    - The color of the square changes based on the server response:
        - **Green** if the response is "1".
        - **Blue** if the response is "0".
        - **Red** for any other response or if there was an error with the request.

4. **Color Change Timing**:
    - The color of the square only changes after it stops moving, ensuring it reflects the response accurately.
