EARS Specs for Hotel Booking Demo

Reservation Flow
	1.	Event-driven: When a guest selects a plan and clicks Reserve room, the system shall display the reservation form for that plan.
	2.	Ubiquitous: The system shall require the guest to provide check-in date, stay duration, number of guests, name, and confirmation type before confirming a reservation.
	3.	Unwanted behavior: If a guest attempts to confirm a reservation without filling a mandatory field, the system shall display a validation error and prevent submission.
	4.	State-driven: While the stay duration exceeds 9 nights, the system shall prevent confirmation and notify the guest of the maximum stay policy.

⸻

Pricing and Calculation
	5.	Event-driven: When a guest selects a weekend check-in date, the system shall apply a 25% surcharge to the base plan price.
	6.	Event-driven: When a guest selects one or more additional plans (e.g., Breakfast, Early check-in, Sightseeing), the system shall increase the total price by $10 per guest per option.
	7.	Ubiquitous: The system shall calculate and display the total cost dynamically as the guest modifies reservation inputs.

⸻

User Experience
	8.	Optional feature: Where a plan includes a recommended tag, the system shall display it prominently at the top of the plan list.
	9.	Event-driven: When a guest confirms a reservation, the system shall display a success message with booking details.
	10.	Unwanted behavior: If the check-in date is more than 3 months in the future, the system shall reject the reservation and display an error message.

⸻

Edge Cases & Data Validation
	11.	Unwanted behavior: If the number of guests is less than 1 or greater than 9, the system shall reject the reservation with an appropriate message.
	12.	Unwanted behavior: If the name field contains invalid characters (e.g., special symbols), the system shall prompt the guest to re-enter a valid name.
	13.	Optional feature: Where the “Special request” field is filled, the system shall include the request text in the booking confirmation details.