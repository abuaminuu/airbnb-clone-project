AIRBNB-CLONE-PROJECT

Overview
Objective: The backend for the Airbnb Clone project is designed to provide a robust and scalable foundation for managing user interactions, property listings, bookings, and payments. This backend will support various functionalities required to mimic the core features of Airbnb, ensuring a smooth experience for users and hosts.

Goal: to get aquainted with the architectural complexity and functionality of the popular booking app airbnb through completion of the following tasks.

1. User Management: implement a secure system for user registration, authentication and profile management.
2. Property Management: develop features for property listing creation, updates and retireval. 
3. Booking System: creating booking mechanism for users, to reserve properties, and manage booking details.
4. Payment Processing: intgerate payment system to handle transaction and record payement details.
3. Review System: allows users to leave reviews and ratings for properties
5. Data Optimization: ensure efficient data retrievaland storage through database optimizations

Tech Stack
1. Django: A high-level Python web framework used for building the RESTful API and web applications.
2. Django REST Framework: Provides tools for creating and managing RESTful APIs.
3. PostgreSQL: A powerful relational database used for data storage.
4. GraphQL: Allows for flexible and efficient querying of data in the database.
5. Celery: For handling asynchronous tasks such as sending notifications or processing payments.
6. Redis: Used for caching and session management.
7. Docker: Containerization tool for consistent development and deployment environments.
8. CI/CD Pipelines: Automated pipelines for testing and deploying code changes.


👥 Team Roles
Backend Developer: Responsible for implementing API endpoints, database schemas, and business logic.
Database Administrator: Manages database design, indexing, and optimizations.
DevOps Engineer: Handles deployment, monitoring, and scaling of the backend services.
QA Engineer: Ensures the backend functionalities are thoroughly tested and meet quality standards.


Database Design

key entities required for the project:
entity: fields ---> relations
Users: id, username, password, email --> user can have multiple property, book multiple properties, can review/rate a property, pay for property, recieve payment.
Properties: id, name, --> property is own by only one user
Bookings: id, booking details --> user who owns the booked a property 
Reviews: id, property_reviewed 
Payments: id amount sender, reciever


