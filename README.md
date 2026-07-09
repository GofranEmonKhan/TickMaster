#  TicketMaster

A web-based event ticket booking and management system built with **Flask** and **PostgreSQL**. The platform allows users to browse events, book tickets, manage bookings, and access a ticket resale marketplace, while providing administrators with tools to manage events and monitor the system.

## ✨ Features

### User

* User registration & login
* Browse available events
* View event details
* Book event tickets
* Checkout system
* View booking history
* Digital ticket page
* Ticket resale marketplace

### Admin

* Admin dashboard
* Create and manage events
* View reports
* Manage resale requests

---

##  Tech Stack

* **Backend:** Flask (Python)
* **Database:** PostgreSQL
* **Frontend:** HTML, CSS, JavaScript (Jinja2 Templates)
* **Authentication:** Werkzeug Password Hashing

---

##  Project Structure

```text
TicketMaster/
│
├── app.py
├── config.py
├── requirements.txt
├── schema.sql
│
├── routes/
|   ├── _init_.py
│   ├── admin.py
│   ├── auth.py
│   ├── booking.py
│   ├── events.py
│   └── resale.py
│
├── templates/
|   ├── base.py
|   ├── index.py
│   ├── admin/
│   ├── auth/
│   ├── booking/
│   ├── events/
│   └── resale/
│
├── static/
│   ├── css/
│   └── js/
│
└── utils.py
```

---

##  Installation

1. Clone the repository.

```bash
git clone <repository-url>
cd TicketMaster
```

2. Create a virtual environment.

```bash
python -m venv venv
```

3. Activate the virtual environment.

Windows:

```bash
venv\Scripts\activate
```

Linux/macOS:

```bash
source venv/bin/activate
```

4. Install dependencies.

```bash
pip install -r requirements.txt
```

5. Create the PostgreSQL database and import the schema.

```bash
psql -U postgres -d ticketmaster -f schema.sql
```

6. Configure environment variables in the `.env` file.

7. Run the application.

```bash
python app.py
```

---

##  Dependencies

* Flask
* Psycopg
* Psycopg Pool
* Werkzeug
* python-dotenv
* Gunicorn

---

##  License

This project was developed for educational purposes.
