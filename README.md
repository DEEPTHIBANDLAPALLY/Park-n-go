# ParkNGO: Vehicle Parking Management System

**ParkNGO** is a Python-based parking management system that enables efficient management of vehicle parking in a structured manner. The system tracks vehicles entering and exiting the parking lot, manages available spaces, and generates parking bills based on the vehicle type and parking duration. It supports multiple vehicle types, including **Bikes**, **Cars**, and **Buses**.

---

## Features

- **Vehicle Entry**: Register new vehicles in the system by entering details such as Vehicle Number, Type (Bike, Car, Bus), Vehicle Name, Owner Name, Date, and Time.
- **Remove Vehicle Entry**: Remove a vehicle from the system by its Vehicle Number.
- **View Parked Vehicles**: View a list of all currently parked vehicles along with their details such as Vehicle Number, Type, Name, Owner, Date, and Time.
- **View Available Parking Spaces**: Display the available parking slots for each vehicle type (Bike, Car, Bus).
- **Parking Rate Information**: Show parking charges per hour for different vehicle types:
  - **Bus**: Rs. 20 per hour
  - **Bike**: Rs. 40 per hour
  - **Car**: Rs. 60 per hour
- **Generate Parking Bill**: Generate and display a bill for the vehicle based on the number of hours parked, including an additional 18% charge.
- **Exit Program**: Gracefully terminate the program.

---

## Requirements

- **Python 3.x**: The system is built using Python 3 and requires no additional libraries.
- No external libraries or dependencies are required, as the program relies on Python's built-in functionality.

---

## Installation

1. **Clone the Repository**:
   - Clone the repository to your local machine by running:
     ```bash
     git clone https://github.com/your-username/ParkNGO.git
     ```

2. **Navigate into the Project Directory**:
   - Change into the directory containing the project:
     ```bash
     cd ParkNGO
     ```

3. **Run the Python Script**:
   - Run the `parkngo.py` script:
     ```bash
     python parkngo.py
     ```

   The program will start running, and you will see a menu to interact with the system.

---

## How to Use

Once the program is running, you will be presented with a menu that provides several options. Below is a detailed breakdown of the available options:

### 1. **Vehicle Entry**
   - The user is prompted to enter the **vehicle number** (in the format `XXXX-XX-XXXX`).
   - The **vehicle type** is selected (`Bus=A`, `Bike=B`, `Car=C`).
   - Then, the user is asked to enter the **vehicle name** and **owner name**.
   - The **date** and **time** of entry are also recorded.

### 2. **Remove Vehicle Entry**
   - The user can remove a vehicle by entering the **vehicle number**.
   - The system will delete the record of the vehicle from the parking database.

### 3. **View Parked Vehicles**
   - Displays a list of all vehicles currently parked, showing:
     - Vehicle Number
     - Vehicle Type
     - Vehicle Name
     - Owner Name
     - Date and Time of Entry

### 4. **View Available Parking Spaces**
   - Displays the number of available spaces for each vehicle type:
     - Available spaces for **Bikes**
     - Available spaces for **Cars**
     - Available spaces for **Buses**

### 5. **Amount Details**
   - Displays the parking rates for each vehicle type:
     - **Bus**: Rs. 20/hour
     - **Bike**: Rs. 40/hour
     - **Car**: Rs. 60/hour

### 6. **Generate Bill**
   - The user is prompted to enter the **vehicle number**.
   - The program calculates the bill based on how long the vehicle has been parked.
   - The total parking charge is calculated along with an **18% service charge**, and the final amount is displayed.

### 7. **Close Program**
   - Exits the program and terminates the session.

---

## Code Structure

### Main Program Logic:
The system runs inside a loop where the user can choose one of the following options:
- Add a vehicle (`Vehicle Entry`)
- Remove a vehicle (`Remove Entry`)
- View parked vehicles (`View Parked Vehicle`)
- View available spaces (`View Left Parking Space`)
- View parking rate (`Amount Details`)
- Generate a bill (`Bill`)
- Close the program (`Close Programme`)

The system uses global variables to store details about parked vehicles, including:
- `Vehicle_Number`: List of vehicle numbers
- `Vehicle_Type`: List of vehicle types corresponding to each vehicle
- `vehicle_Name`: List of vehicle names
- `Owner_Name`: List of owner names
- `Date`: List of dates of vehicle entries
- `Time`: List of entry times for each vehicle

### Parking Space Tracking:
The system tracks the available parking spaces for each vehicle type:
- **Bikes**: 100 spaces
- **Cars**: 250 spaces
- **Buses**: 78 spaces

### Error Handling:
The program includes basic validation for user input to ensure that vehicle numbers, dates, and times are valid. It will prompt the user again if the input is invalid.

---

## Example Workflow

### 1. **Vehicle Entry**
   - The user enters a vehicle number: `AB12-CD-1234`.
   - Selects the type as `Bike`.
   - Enters the vehicle name as `Intruder` and owner as `John Doe`.
   - Provides the date and time of entry, e.g., `01-01-2025` and `10:30:00`.

### 2. **Generate Bill**
   - The user enters the vehicle number `AB12-CD-1234`.
   - The program calculates the bill based on how long the bike has been parked.
   - It displays the total parking charge along with the service charge.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Contributing

Contributions are welcome! If you find any bugs, want to suggest improvements, or add new features, feel free to open an issue or submit a pull request. You can contribute by:
- Reporting bugs or issues.
- Adding features or enhancements.
- Improving the documentation.

---

## Acknowledgments

- This project is built with **Python 3** and uses standard libraries like `time` for handling date and time inputs.
- Thanks to the open-source community for providing resources that helped in building this system.

---

Feel free to modify the project as per your requirements. Enjoy using **ParkNGO**!
