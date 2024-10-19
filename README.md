
# Polling-app-django

This is a full-featured polling application where users can register, view polls, and vote on them. The app ensures that users can vote only once per poll, and only the poll owner can create, update, or delete polls and their choices. Polls can be ended by the owner, after which no voting can take place, and only the final results are shown.

# Features

- User Registration and Authentication: Users need to register to view polls and vote.
- Vote Restriction: Users can only vote once per poll.
- Poll Management: Poll owners can create, edit, update, delete polls and choices.
- End Polls: Polls can be ended by the owner, showing only the final results to users.
- Search and Filters: Users can search for polls and filter by name, publish date, and number of votes.
- Pagination: Works with filters applied.
  
# Getting Started
Follow these instructions to set up the project on your local machine for development and testing.

# Prerequisites
Ensure that the following are installed on your machine:
- Python 3.5 or later
- Django 2.0 or later

# Installation
1. Clone the repository using Git:
2. 2. Navigate to the project directory:
3. Install the required packages:
4. Apply the migrations to set up the database:
   python manage.py makemigrations
   python manage.py migrate
   

# Creating a Superuser (For Admin Access)
To access the Django admin panel, create a superuser:
python manage.py createsuperuser


# Dummy Data Setup (Optional)
You can create some dummy data for testing purposes using the following commands:

1. Install the Faker package:
   pip install faker
   

2. Generate 30 dummy entries (you can change the number):
   python manage.py shell
   from seeder import seed_all
   seed_all(30)

# Running the Application

Start the Django development server:
python manage.py runserver

Then open your browser and navigate to:
http://127.0.0.1:8000

# Polls Management

- Only the poll owner can create, update, delete polls and choices.
- Polls can be ended, after which no more votes can be cast, and the final result is displayed.
- Users can search polls by name, and filter by publish date or number of votes.
