# BoxConstructor

## Project Description

BoxConstructor is a desktop application for managing box manufacturing orders and calculating production costs and financial outcomes. The application allows users to create, edit, and manage custom box orders with different materials, dimensions, and quantities, while automatically calculating costs, revenues, and business expenses.

## Purpose

This project was developed as a university coursework assignment for Object-Oriented Programming (OOP) course in Semester 3. It demonstrates:

- Object-oriented design principles
- GUI application development
- File I/O operations
- Business logic implementation
- Exception handling
- Data management and sorting

## Technologies Used

### Core Technologies
- **C++17** - Primary programming language
- **Qt 6.8.0** - GUI framework for cross-platform desktop application development
- **CMake 3.16+** - Build system and project configuration

### Qt Modules
- **Qt Widgets** - GUI components (windows, dialogs, tables, buttons)
- **Qt Core** - Core non-GUI functionality
- **Qt GUI** - GUI-related classes

### Development Tools
- **LLVM/MinGW 64-bit** - Compiler toolchain
- **Qt Creator** - IDE (optional)

## Features

- **Order Management**
  - Add new box orders with custom dimensions (length, width, height)
  - Edit existing orders
  - Delete orders
  - View all orders in a table format

- **Material Selection**
  - Corrugated Cardboard
  - Solid Cardboard
  - Wood
  - Biodegradable materials
  - Plastic

- **Cost Calculations**
  - Automatic material cost calculation based on box dimensions
  - Customizable material pricing
  - Order cost computation
  - Total materials cost

- **Financial Management**
  - Monthly income calculation
  - Business outcomes tracking (salaries, taxes, communal services, amortization)
  - Profit/loss analysis

- **Data Persistence**
  - Save orders to file
  - Load orders from file
  - Export results

- **Sorting & Organization**
  - Sort orders by various criteria
  - Table-based visualization

## Project Structure

```
BoxConstructor/
├── main.cpp              # Application entry point
├── mainwindow.cpp/h/ui   # Main window implementation and UI
├── dialog.cpp/h/ui       # Add/Edit dialog implementation and UI
├── order.cpp/h           # Order and MonthlyRecord classes
├── exceptions.h          # Custom exception definitions
├── CMakeLists.txt        # CMake build configuration
├── app-icon.rc           # Application icon resource
├── december_orders.txt   # Sample orders data
└── build/                # Build artifacts directory
```

## Building the Project

### Prerequisites
- Qt 6.8.0 or later
- CMake 3.16 or later
- C++17 compatible compiler (LLVM/MinGW, GCC, MSVC)

### Build Steps

1. Clone or download the repository

2. Create a build directory:
```bash
mkdir build
cd build
```

3. Configure with CMake:
```bash
cmake ..
```

4. Build the project:
```bash
cmake --build .
```

5. Run the executable:
```bash
./BoxConstructor  # Linux/macOS
BoxConstructor.exe  # Windows
```

### Using Qt Creator

1. Open `CMakeLists.txt` in Qt Creator
2. Configure the project with your Qt kit
3. Build and run using the IDE controls

## Usage

1. **Adding Orders**: Click the "Add" button to create a new box order with specified dimensions, material, and quantity
2. **Editing Orders**: Select an order from the table and click "Edit" to modify its parameters
3. **Deleting Orders**: Select an order and click "Delete" to remove it
4. **Calculating Costs**: Use the cost calculation buttons to view material costs and order totals
5. **Financial Analysis**: Calculate monthly income and business outcomes (salaries, taxes, etc.)
6. **Managing Prices**: Modify material prices in the pricing table as needed
7. **Sorting**: Use the sort button to organize orders by different criteria
