[README.md](https://github.com/user-attachments/files/29512422/README.md)
# UTM Peer Tutoring & Skill Exchange Assistant

SECV2223 Web Programming Final Project - Group 8 (Cybernetics)

## Main features
- Registration and secure login for learner, tutor, and administrator roles.
- Tutor listing CRUD with subject, description, price, mode, location, and availability.
- Search, filter, and sort tutor listings.
- Booking request workflow: pending, accepted, rejected, cancelled, and completed.
- Ratings and reviews after completed sessions.
- Admin management for users, subjects, bookings, and reviews.
- Responsive Bootstrap interface and JavaScript validation.
- Internal tutor recommendation assistant and Google Calendar event link.
- Prepared SQL statements, password hashing, CSRF tokens, output escaping, and access-control checks.

## Local setup using XAMPP
1. Start Apache and MySQL in XAMPP.
2. Copy the `UTM_Peer_Tutoring` folder into `htdocs`.
3. Open phpMyAdmin and import `database/schema.sql`.
4. Open `config/config.php` and confirm the database settings.
5. If the folder name changes, update `BASE_URL`.
6. Open `http://localhost/UTM_Peer_Tutoring/`.

## Demo accounts
All demo accounts use password: `Student123!`
- Admin: `admin@utm.my`
- Tutor: `aiman@graduate.utm.my`
- Learner: `learner@graduate.utm.my`

## Notes
- The recommendation assistant is implemented locally with PHP/MySQL so the project runs without an external paid service. It can later be replaced with Botpress.
- The Calendar button opens a prepared Google Calendar event. No API key is required.
- Email delivery is not enabled because local XAMPP normally has no mail server. The system uses in-app notifications.
