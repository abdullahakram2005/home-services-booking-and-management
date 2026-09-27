# Software Requirements Specification
## Home Services Booking & Management System

## 1. Introduction

The Home Services Booking & Management System is a full-stack web application that provides a platform for customers to find and book professional home services. The system connects customers with service providers such as electricians, plumbers, AC technicians, cleaners, and other home maintenance professionals.

The application will provide separate functionality for customers, service providers, and administrators.


## 2. Problem Statement

Finding reliable home service providers can be difficult and time-consuming. Customers usually have to search for service providers through different sources and contact them manually.

The proposed system will provide a centralized platform where customers can easily find available services, select service providers, book appointments, and track their booking status.


## 3. Objectives

The main objectives of the system are:

- Provide an easy platform for booking home services.
- Connect customers with service providers.
- Allow customers to search and filter available services.
- Allow customers to book services according to their preferred date and time.
- Allow service providers to manage booking requests.
- Provide booking status tracking.
- Allow customers to rate and review completed services.
- Provide an admin panel for managing the overall system.
- Maintain records of users, services, bookings, and reviews.


# 4. Users of the System

The system will have three main users.

## 4.1 Customer

A customer can:

- Register an account.
- Login and logout.
- Manage their profile.
- Browse available services.
- Search for services.
- Filter services by category.
- View service provider information.
- Book a service.
- Select date and time.
- View booking status.
- Cancel a booking.
- View booking history.
- Give ratings and reviews.

## 4.2 Service Provider

A service provider can:

- Register as a service provider.
- Login and logout.
- Create and manage their profile.
- Select service categories.
- Add service information.
- Set service charges.
- Manage availability.
- View booking requests.
- Accept or reject booking requests.
- Update booking status.
- View completed bookings.
- View booking history.

## 4.3 Administrator

An administrator can:

- Login to the admin panel.
- Manage customers.
- Manage service providers.
- Approve or reject service providers.
- Add service categories.
- Update service categories.
- Delete service categories.
- Manage bookings.
- Manage reviews and ratings.
- Monitor system activities.


# 5. Functional Requirements

## FR-01: User Registration

The system shall allow customers and service providers to create an account.

## FR-02: User Login

The system shall allow registered users to login using their credentials.

## FR-03: Role-Based Access

The system shall provide different access and functionality based on the user's role.

Roles:

- Customer
- Service Provider
- Admin

## FR-04: Service Browsing

Customers shall be able to view available home services.

## FR-05: Service Search

Customers shall be able to search for specific services.

## FR-06: Service Filtering

Customers shall be able to filter services according to categories.

## FR-07: Provider Profiles

Customers shall be able to view service provider information such as:

- Name
- Experience
- Services
- Location
- Charges
- Rating

## FR-08: Service Booking

Customers shall be able to book a service by selecting:

- Service
- Service provider
- Date
- Time
- Address
- Additional requirements

## FR-09: Booking Management

Customers shall be able to view their bookings and booking status.

## FR-10: Booking Status

The system shall support the following booking statuses:

- Pending
- Accepted
- Rejected
- In Progress
- Completed
- Cancelled

## FR-11: Provider Booking Management

Service providers shall be able to:

- View booking requests.
- Accept bookings.
- Reject bookings.
- Update booking status.

## FR-12: Booking History

Customers and service providers shall be able to view their previous bookings.

## FR-13: Reviews and Ratings

Customers shall be able to provide ratings and reviews after a completed service.

## FR-14: Admin User Management

The administrator shall be able to manage registered customers and service providers.

## FR-15: Admin Service Management

The administrator shall be able to add, update, and remove service categories.

## FR-16: Admin Booking Management

The administrator shall be able to view and monitor bookings.

## FR-17: Profile Management

Users shall be able to update their profile information.


# 6. Non-Functional Requirements

## Performance

The system should respond to normal user requests within a reasonable amount of time.

## Security

- User passwords should be securely hashed.
- Authentication should be implemented.
- Users should only access functionality permitted by their role.
- Sensitive information should not be exposed.

## Usability

The interface should be simple and easy to understand.

## Responsiveness

The application should work properly on:

- Desktop
- Tablet
- Mobile

## Reliability

The system should maintain accurate booking and user information.

## Maintainability

The project should use a modular code structure so that new features can be added easily.

## Scalability

The system should be designed so that additional services and users can be added in the future.


# 7. Technology Requirements

## Frontend

- React.js
- JavaScript
- HTML5
- CSS3
- Tailwind CSS

## Backend

- Node.js
- Express.js

## Database

- MongoDB

## Authentication

- JWT
- Password hashing

## Development Tools

- Visual Studio Code
- Git
- GitHub
- Postman

# 8. Main Modules

The system will consist of the following major modules:

1. Authentication Module
2. Customer Module
3. Service Provider Module
4. Service Management Module
5. Booking Module
6. Review and Rating Module
7. Admin Module

# 9. Future Enhancements

The system can be extended with:

- Online payments
- Google Maps/location integration
- Real-time notifications
- Customer-provider chat
- Mobile application
- Advanced search
- Service recommendations
- Email/SMS notifications
