# Link Collector

This project is a simple Django web application that allows users to input a website URL, scrape its content for links, and display them. Users can also delete all collected links.

## Getting Started

To run this project locally, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/your_username/link-collector.git
   ```

2. Install the required dependencies. It's recommended to use a virtual environment:

   ```bash
   cd link-collector
   pip install -r requirements.txt
   ```

3. Run migrations to set up the database:

   ```bash
   python manage.py migrate
   ```

4. Start the Django development server:

   ```bash
   python manage.py runserver
   ```

5. Open your web browser and go to `http://127.0.0.1:8000/` to access the application.

## Usage

1. Enter a website address in the provided input field and click on the "Scrape" button to scrape the website for links.
2. The collected links will be displayed in a table format below the input field.
3. To delete all collected links, click on the "Delete" button.

## Technologies Used

- **Django**: The web framework used to build the application.
- **Bootstrap**: Frontend framework for styling the user interface.
- **Beautiful Soup**: Python library for web scraping.
- **Requests**: Python library for making HTTP requests.

## Project Structure

- **`myapp/`**: Contains the Django application files.
  - **`models.py`**: Defines the database models, including the `Link` model for storing scraped links.
  - **`views.py`**: Contains the view functions for rendering HTML templates and handling form submissions.
  - **`result.html`**: HTML template for displaying the main page with the input form and the list of collected links.
- **`README.md`**: Documentation file for the project.
- **`requirements.txt`**: Lists all Python dependencies required to run the project.

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Make your changes.
4. Commit your changes (`git commit -am 'Add some feature'`).
5. Push to the branch (`git push origin feature/your-feature`).
6. Create a new Pull Request.
