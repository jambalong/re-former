# Re-former

This project is part of The Odin Project: [Forms](https://www.theodinproject.com/lessons/ruby-on-rails-forms) in Ruby on Rails Curriculum.

## Overview

Re-former is a Ruby on Rails application designed to demonstrate form handling and user management using Rails forms. The project covers setting up a backend, building HTML forms, and utilizing Rails form helpers.

## Assignment Steps

1. **Set Up the Back End**:
   - Create a new Rails app named `re-former`.
   - Initialize a GitHub repository and connect it to your local repo.
   - Modify the README to include project details.
   - Create a `User` model with fields: `username`, `email`, and `password`, with presence validations.
   - Set up routes for users and create a `UsersController`.
   - Implement `#new` and `#create` actions, and create a view for the new user form.

2. **Build an HTML Form**:
   - Create a form for user registration in `app/views/users/new.html.erb`, ensuring proper method, action, and input fields.
   - Submit the form to verify that parameters are being passed correctly.

3. **Railsy Forms with `#form_tag`**:
   - Replace the HTML form with a Rails form using `#form_tag`.
   - Update the controller to accept normal top-level User attributes.

4. **Railsy-er Forms with `#form_with`**:
   - Modify the controller to instantiate a blank `User` object and use `#form_with` in the new view.
   - Implement nested user parameters for easier attribute handling.

5. **Editing Users**:
   - Update routes and controller for editing user functionality.
   - Create an edit view and adjust the form for PATCH requests.
   - Display error messages for validation failures in the form.

## Installation

To set up the Re-former application locally:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/jambalong/re-former.git
   cd re-former
   ```

2. **Install dependencies**:
   ```bash
   bundle install
   ```

3. **Set up the database**:
   ```bash
   rails db:create
   rails db:migrate
   ```

4. **Start the server**:
   ```bash
   rails server
   ```

Visit `http://localhost:3000/users/new` to access the app.
