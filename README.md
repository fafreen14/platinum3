# Restaurant Reservation System

## Overview
This project implements a simple reservation system for a restaurant. It allows users to make, change, view, and cancel reservations.

## Contributors
- **Fnu Afreen**:
  - Implemented the `RestaurantReservation` class with methods to manage reservations:
    - `__init__(self)`: Constructor that initializes an instance of the class with an empty dictionary for storing reservations.
    - `make_reservation(self, name, time, date)`: Adds a reservation for a given name, time, and date to the reservations dictionary and prints a confirmation message.
    - `change_reservation(self, name, new_time, new_date)`: Modifies an existing reservation, identified by the customer’s name, to a new time and date if it exists. It prints an updated confirmation or an error if the reservation doesn’t exist.
    - `get_reservation(self, name)`: Prints details of a specific reservation if it exists; otherwise, it prints an error message.
    - `cancel_reservation(self, name)`: Removes a reservation from the dictionary if it exists and confirms the cancellation, or notifies if no such reservation is found.

- **Abdulfaruq Seriki**:
  - Developed the interactive menu loop for the command-line interface:
    - The code provides a loop that displays a menu with options to make, change, view, or cancel a reservation, or exit the program.
    - Depending on the user’s choice, it prompts for the necessary details (name, date, and time) and calls the appropriate method in the `RestaurantReservation` class.
    - The loop continues until the user chooses to exit.

## Usage
To use the program, run the main script and follow the on-screen prompts to interact with the reservation system. Choose from making a reservation, changing an existing one, viewing details of a reservation, canceling a reservation, or exiting the program.

## License
This project is open-sourced under the MIT license.
