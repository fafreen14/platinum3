def make_reservation(self, name, time, date):
        self.reservations[name] = {'time': time, 'date': date}
        print(f"Reservation made for {name} on {date} at {time}.")

def change_reservation(self, name, new_time, new_date):
        if name in self.reservations:
            self.reservations[name]['time'] = new_time
            self.reservations[name]['date'] = new_date
            print(f"Reservation for {name} changed to {new_date} at {new_time}.")
        else:
            print(f"Reservation '{name}' not found.")

def get_reservation(self, name):
        if name in self.reservations:
            reservation = self.reservations[name]
            print(f"Reservation for {name}: {reservation['date']} at {reservation['time']}")
        else:
            print(f"Reservation '{name}' not found.")

def cancel_reservation(self, name):
        if name in self.reservations:
            del self.reservations[name]
            print(f"Reservation for {name} has been canceled.")
        else:
            print(f"Reservation '{name}' not found.")

            ** Part 1 of Code by Fnu Afreen

      restaurant = RestaurantReservation()
while True:
    print("\nOptions:")
    print("1. Make a reservation")
    print("2. Change a reservation")
    print("3. View a reservation")
    print("4. Cancel a reservation")
    print("5. Exit")
    choice = input("Choose an option: ")

    if choice == "1":
        name = input("Enter the customer's name: ")
        time = input("Enter the time of the reservation (HH:MM): ")
        date = input("Enter the date of the reservation (YYYY-MM-DD): ")
        restaurant.make_reservation(name, time, date)
    elif choice == "2":
        name = input("Enter the customer's name whose reservation is to be changed: ")
        new_time = input("Enter the new time of the reservation (HH:MM): ")
        new_date = input("Enter the new date of the reservation (YYYY-MM-DD): ")
        restaurant.change_reservation(name, new_time, new_date)
    elif choice == "3":
        name = input("Enter the customer's name to view the reservation: ")
        restaurant.get_reservation(name)
    elif choice == "4":
        name = input("Enter the customer's name to cancel the reservation: ")
        restaurant.cancel_reservation(name)
    elif choice == "5":
        print("Exiting...")
        break
    else:
        print("Invalid option. Please try again.")

        ** Part 2 of the code by Abdulfaruq Seriki
