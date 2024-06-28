## Flask Application Design

### HTML Files

- **index.html**: This file will serve as the main page of the web application and will guide the user through the club fitting process. It will contain various elements, such as:
    - Welcome message and instructions
    - Form for user to input their information (e.g., height, weight, swing speed)
    - Button to submit the information and initiate the club fitting

- **results.html**: This file will display the results of the club fitting, including the recommended golf clubs based on the user's input. It may also provide additional information or recommendations.

### Routes

- **@app.route('/', methods=['GET', 'POST'])**: This route will handle the main page ("/").
    - **GET**: This will render the **index.html** file, displaying the welcome message and form.
    - **POST**: This will capture the user's input from the form and pass it on to the club fitting AI agent. It will then redirect the user to the results page.

- **@app.route('/results', methods=['GET'])**: This route will handle the results page ("/results").
    - **GET**: This will render the **results.html** file, displaying the recommended golf clubs based on the user's input.