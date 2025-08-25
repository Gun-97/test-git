Asset Central: A C++ Stock Management System
🌟 Introduction
Asset Central is a powerful command-line application built in C++ to help manage and track inventory. It provides a robust system for administrators and staff to handle stock, user accounts, and sales transactions. The system uses Excel files for data persistence, making it easy to manage and report on your asset data.

📦 Features
User Management: Secure login system with separate roles for administrators and general staff.

Stock Management:

Add, update, and delete stock items.

View all stock items with detailed information (ID, name, quantity, price).

Search for specific stock items.

Transaction Logging: Records all sales transactions into a receipt log.

Data Persistence: Uses the xlnt library to read and write all user, stock, and receipt data to Excel (.xlsx) files.

Clean Interface: Utilizes the tabulate library to display information in clean, easy-to-read tables on the command line.

🛠️ Prerequisites
To build and run this project, you will need:

A C++ compiler that supports the C++17 standard (e.g., GCC, Clang, MSVC).

CMake (version 3.14 or higher) to handle the build process and dependencies.

A compatible operating system (tested on Windows and Linux).

The project's CMakeLists.txt file will automatically download the necessary xlnt and tabulate libraries.

🚀 Build Instructions
Follow these steps to build the project from source:

Clone the repository:

git clone https://github.com/your-username/asset-central.git
cd asset-central


Create a build directory and run CMake:

mkdir build
cd build
cmake ..


Build the project:

On Windows (using Visual Studio): Open the generated .sln file and build from there.

On Linux or macOS (using Make):

make


The executable will be generated in the build directory.

🖥️ Usage
After building, you can run the application from the build directory.

# On Linux/macOS
./StockManagementSystem

# On Windows
StockManagementSystem.exe


The application will launch a command-line interface, prompting you to log in or register.

📁 File Structure
src/: Contains all the C++ source files (.cpp).

include/: Contains all the C++ header files (.hpp).

data/: The directory where the application will store its Excel data files (users.xlsx, stocks.xlsx, etc.) at runtime.

CMakeLists.txt: The build script for CMake.

🤝 Contributing
Contributions are welcome! If you have suggestions or find a bug, please open an issue or submit a pull request.
