
# Movie Theater Ticket Kiosk

## Project Description

The Movie Theater Ticket Kiosk is a simple self-service system that allows customers to view available movies and showtimes, select an available seat, and purchase a ticket. After a successful purchase, the system provides a confirmation. The system also prevents the same seat from being sold twice.

## Main Requirements

1. A customer can view available movies and showtimes.
2. A customer can choose an available seat.
3. A customer can purchase a ticket.
4. The system provides a confirmation after a successful purchase.
5. The system must prevent the same seat from being sold twice.

## UML Diagrams

The diagrams folder contains the UML diagrams created for the Movie Theater Ticket Kiosk.

### Domain Model

The domain model contains the main concepts of the system, including:

- Customer
- Movie
- Showtime
- Seat
- Ticket
- Payment

The model shows the important relationships between these concepts.

### Use Case Diagram

The use-case diagram contains the Customer actor and the following main use cases:

- View Showtimes
- Select Seat
- Purchase Ticket

## Expanded Use Case: Purchase Ticket

**Primary Actor:** Customer

**Precondition:** The customer has selected a movie and showtime, and tickets are available.

### Main Steps

1. The customer views the available seats.
2. The customer selects an available seat.
3. The system checks whether the selected seat is available.
4. The customer confirms the ticket selection.
5. The customer provides payment information.
6. The system processes the payment.
7. The system creates the ticket.
8. The system displays the purchase confirmation.

**Postcondition:** The ticket is successfully purchased, the selected seat is reserved, and the customer receives a confirmation.

## Sequence Diagram

The Purchase Ticket sequence diagram shows the interaction between the Customer, Kiosk Interface, Ticket Service, and Payment Service.

The sequence includes:

1. Customer selects a showtime.
2. Kiosk Interface requests available seats.
3. Ticket Service returns available seats.
4. Customer selects a seat.
5. Kiosk Interface requests the Ticket Service to check seat availability.
6. Ticket Service requests payment processing.
7. Payment Service confirms successful payment.
8. Ticket Service confirms the purchase.
9. Kiosk Interface displays the confirmation to the customer.

## Repository Contents

- `README.md` - Project description and expanded use case.
- `requirements.md` - Movie Theater Ticket Kiosk requirements.
- `diagrams/` - UML diagram source files and PNG exports.

## Tools Used

- GitHub - Repository, version control, issues, and project board.
- diagrams.net (draw.io) - UML domain model, use-case diagram, and sequence diagram.
