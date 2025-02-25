# FlavorGraph - A Recipe Search Application

FlavorGraph is a Python web application designed to help users discover and search for recipes based on the ingredients they have on hand. The application provides a user-friendly interface that allows users to input ingredients and fetch matching recipes from a database. It also includes features for viewing all available recipes and searching by multiple ingredients, making it a versatile tool for home cooks and food enthusiasts.

## Project Structure

```
FlavorGraph/
├── backend/                     # Backend directory (FastAPI application)
│   ├── __pycache__/             # Compiled Python files (auto-generated)
│   ├── static/                  # Static files (CSS, images, etc.)
│       ├── styles.css           # CSS file for backend-related styling
│   ├── __init__.py              # Marks this directory as a Python package
│   ├── main.py                  # FastAPI application entry point
│   ├── recipes.csv              # CSV file containing recipe data
├── frontend/                    # Frontend directory (Static website)
│   ├── index.html               # Main HTML file for the frontend
├── .gitignore                   # Git ignore file (ignore unnecessary files)
├── README.md                    # Instructions for running the project

```

## Requirements and Dependencies

- Python 3.x
- FastAPI
- Uvicorn
- Pandas
- Additional libraries as needed for future features

## Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   cd FlavorGraph/backend
   ```

2. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

## Running the Application

1. Start the FastAPI server:
   ```
   uvicorn backend.main:app --reload
   ```

2. Open your browser and navigate to `http://127.0.0.1:8000`.

3. Use the search bar to input ingredients and fetch matching recipes or click "View All Recipes" to see all available recipes.

## Deployment and Hosting

For deployment, you can use platforms like Render, Vercel, or Heroku. Follow their respective documentation for deployment instructions.

## Notes

- The application strictly relies on the CSV file for data.
- Ensure the CSV file is formatted correctly with the required columns: Recipe Name, Ingredients, Steps.

## Data Structures and Algorithms

- **Data Structure**: The application uses a CSV file to store recipe data, which is structured in a tabular format.
- **Algorithm**: The application likely employs search algorithms to filter recipes based on user input (ingredients), although specific implementations are not detailed in the documentation.
