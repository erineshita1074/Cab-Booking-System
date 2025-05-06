# Cab-Booking-System
This Java-based Cab Booking System is a simple, console-driven application that enables users to register, log in, book cabs, and view their booking history. It serves as a practical implementation of Object-Oriented Programming (OOP) concepts such as abstraction, encapsulation, inheritance, and polymorphism.

At the core of the system is the Vehicle abstract class, which defines common attributes and behaviors for all types of vehicles, such as cab ID, type, and availability status. The Cab class inherits from Vehicle and implements the Bookable interface, providing concrete functionality to display cab details and handle cab bookings.

The Bookable interface defines a method bookCab() which is implemented by the Cab class to perform the actual booking logic. When a cab is booked, its availability is set to false, and a booking record is created.

The Booking class encapsulates details about each booking, including the booking ID, user name, selected cab, pickup and drop locations, and the booking time. It overrides the toString() method to neatly display booking information.

The main controller class, CabBookingSystem, manages users, cabs, and bookings. It uses arrays to store cab and booking objects, and a HashMap to maintain registered users along with their passwords. The system allows up to four cabs and ten bookings for simplicity.

Users can interact with the system via a menu that offers the following options:

Register a new account

Log in to an existing account

Log out

View all available cabs

Book a cab by specifying the cab ID and locations

View their booking history

Exit the system

The system checks for user authentication before allowing cab booking or viewing booking history. It also ensures that only available cabs can be booked and prevents overbooking beyond the set limit.

This project demonstrates effective use of OOP and is suitable for beginners learning how to structure interactive, multi-class applications in Java.
