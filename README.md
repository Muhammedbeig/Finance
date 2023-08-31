# CS50 Finance Project Readme


Welcome to the CS50 Finance project! This project is a part of the CS50 curriculum and is designed to help you understand the concepts of web development, databases, and financial interactions.

## Project Overview

CS50 Finance is a web application that simulates a stock trading platform. Users can register, log in, view stock prices, buy and sell stocks, and see their transaction history. The application utilizes the Flask framework for the backend, SQLite for the database, and HTML/CSS for the frontend.

## Installation

1. **Clone the Repository**: Start by cloning this repository to your local machine using the following command:

   ```
   git clone https://github.com/your-username/cs50-finance.git
   ```

2. **Setup Virtual Environment (Optional but Recommended)**: It's a good practice to create a virtual environment to isolate project dependencies. Navigate to the project directory and create a virtual environment:

   ```
   cd cs50-finance
   python3 -m venv venv
   ```

   Activate the virtual environment:

   - On macOS and Linux:

     ```
     source venv/bin/activate
     ```

   - On Windows:

     ```
     venv\Scripts\activate
     ```

3. **Install Dependencies**: Install the required dependencies using pip:

   ```
   pip install -r requirements.txt
   ```

4. **Database Configuration**: The application uses an SQLite database to store user and transaction data. To set up the database, execute the following commands:

   ```
   flask db init
   flask db migrate
   flask db upgrade
   ```

5. **Environment Variables**: Create a `.env` file in the project directory and add the following environment variables:

   ```
   FLASK_APP=application.py
   FLASK_ENV=development
   ```

   Replace `application.py` with the actual name of your Flask application file if it's different.

6. **API Key**: You will need an API key from a stock market data provider (e.g., IEX Cloud) to fetch real-time stock prices. Store this API key in the `.env` file as well:

   ```
   API_KEY=your-api-key
   ```

7. **Run the Application**: You can now run the application using the following command:

   ```
   flask run
   ```

   This will start the development server, and you can access the application by visiting `http://localhost:5000` in your web browser.

## Usage

1. **Register/Login**: Create an account or log in using your credentials.

2. **Quote**: Get real-time stock prices by entering the stock symbol.

3. **Buy**: Purchase stocks by specifying the stock symbol and the number of shares.

4. **Sell**: Sell stocks you own by specifying the stock symbol and the number of shares.

5. **History**: View your transaction history, including buy and sell activities.

## Credits

CS50 Finance was developed as part of the CS50 course at Harvard University. The project template and initial code structure were provided by the CS50 team.

## License

This project is licensed under the MIT License. Feel free to modify and distribute it as needed.

## Acknowledgments

We would like to express our gratitude to the CS50 staff, instructors, and fellow learners for their support and guidance throughout this project.

---

Enjoy exploring the world of web development, databases, and finance with CS50 Finance! If you have any questions or need assistance, feel free to reach out to the CS50 community or the project maintainers. Happy coding! 🚀
