# Flights SQL App ✈️  

The **Flights SQL App** is a database-driven application designed to manage and analyze flight data. It uses **SQL** for querying and managing flight records and provides an intuitive and interactive interface using **Streamlit**.  

---

## Table of Contents  

- [Introduction](#introduction)  
- [Key Features](#key-features)  
- [Tech Stack](#tech-stack)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Database Schema](#database-schema)  
- [Future Enhancements](#future-enhancements)  
- [Contributing](#contributing)  
- [License](#license)  

---

## Introduction  

This project focuses on leveraging **SQL** to handle and analyze flight-related data while offering a user-friendly **Streamlit-based interface** for interacting with the data. Users can query flight schedules, passenger information, and more through a simple web app interface.  

---

## Key Features  

- 🗂️ **Manage flight records** including flight IDs, schedules, and routes.  
- 🛫 **Query passenger data** to check bookings and travel history.  
- 📊 Perform complex **SQL queries** for detailed analysis.  
- 🔍 Filter flights based on **destination, time, or status**.  
- 💾 Interactive and responsive interface using **Streamlit**.  

---

## Tech Stack  

- **Programming Language:** Python 🐍  
- **Database:** MySQL / SQLite  
- **Libraries Used:** SQLAlchemy, Pandas, Streamlit  
- **Visualization Tools:** Matplotlib, Seaborn  

---

## Installation  

### Prerequisites:  
- Python 3.8+  
- A SQL database (MySQL or SQLite)  
- pip (Python package manager)  

### Steps:  

1. Clone the repository:  
   ```bash  
   git clone https://github.com/tarunkumar1111/flights-sql-app.git  
   ```  

2. Navigate to the project directory:  
   ```bash  
   cd flights-sql-app  
   ```  

3. Set up the database:  
   - Import the SQL schema file to your database:  
     ```bash  
     mysql -u username -p database_name < flights_schema.sql  
     ```  

4. Install the required dependencies:  
   ```bash  
   pip install -r requirements.txt  
   ```  

5. Run the Streamlit app:  
   ```bash  
   streamlit run app.py  
   ```  

---

## Usage  

1. Set up your database connection in the `config.py` file.  

2. Run the Streamlit app:  
   ```bash  
   streamlit run app.py  
   ```  

3. Open your browser at the URL provided by Streamlit (usually `http://localhost:8501`).  

4. Use the web app to:  
   - Query flight details and passenger information.  
   - Visualize trends and activity using interactive charts.  
   - Perform custom SQL queries through the interface.  

---

## Database Schema  

The database contains the following key tables:  

- **Flights Table**:  
  - `Flight_ID` (Primary Key)  
  - `Origin`  
  - `Destination`  
  - `Departure_Time`  
  - `Arrival_Time`  

- **Passengers Table**:  
  - `Passenger_ID` (Primary Key)  
  - `Name`  
  - `Flight_ID` (Foreign Key)  
  - `Booking_Status`  

- **Airlines Table**:  
  - `Airline_ID` (Primary Key)  
  - `Airline_Name`  

- **Sample Relationships:**  
  - One flight can have many passengers.  
  - Each flight is operated by one airline.  

---

## Future Enhancements  

- Add **real-time flight status tracking** using APIs.  
- Enable **seat management and pricing models**.  
- Add **advanced visualizations** for flight trends and passenger demographics.  
- Integrate **multi-language support** for a broader audience.  

---

## Contributing  

Contributions are welcome! Follow these steps to contribute:  

1. Fork the repository.  
2. Create a new branch for your feature or bug fix:  
   ```bash  
   git checkout -b feature-name  
   ```  

3. Commit your changes and push them:  
   ```bash  
   git push origin feature-name  
   ```  

4. Open a pull request with a detailed description of your changes.  

---

## License  

This project is licensed under the **MIT License**. Feel free to use it in your own projects.  

---

## Acknowledgments  

- Thanks to Python, SQL, and Streamlit for enabling seamless data management and interactive interfaces.  
- Special appreciation to the open-source community for their resources and inspiration.  
