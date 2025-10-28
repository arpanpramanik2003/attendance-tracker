<!-- Repository Header -->
<div align="center">

# 📊 Attendance Tracker

[![Python Version](https://img.shields.io/badge/python-3.x-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/arpanpramanik2003/attendance-tracker/graphs/commit-activity)
[![GitHub issues](https://img.shields.io/github/issues/arpanpramanik2003/attendance-tracker)](https://github.com/arpanpramanik2003/attendance-tracker/issues)
[![GitHub stars](https://img.shields.io/github/stars/arpanpramanik2003/attendance-tracker)](https://github.com/arpanpramanik2003/attendance-tracker/stargazers)

**A robust Python-based GUI application for streamlined student attendance management**

[Features](#-features) • [Installation](#-installation) • [Usage](#-usage) • [Documentation](#-documentation) • [Contributing](#-contributing)

</div>

---

## 📋 Overview

Attendance Tracker is a lightweight, user-friendly desktop application built with Python and Tkinter that simplifies the process of managing student attendance records. Designed for educators, administrators, and institutions, this tool provides an intuitive interface for registering students, tracking daily attendance, and maintaining historical records in CSV format.

### Why Attendance Tracker?

- 🔒 **Secure Access** - Built-in authentication system to protect sensitive data
- 📅 **Dynamic Date Management** - Automatic date column creation for seamless tracking
- 💾 **Persistent Storage** - Reliable CSV-based data storage
- 🎯 **Simple Interface** - Clean, intuitive GUI designed for ease of use
- ⚡ **Lightweight** - Minimal dependencies, runs on standard Python installations

---

## ✨ Features

### Core Functionality

- **🔐 User Authentication**
  - Secure login system ensuring only authorized access
  - Password-protected entry to attendance management

- **👥 Student Registration**
  - Easy student enrollment with name and unique ID (UID)
  - Duplicate UID validation to maintain data integrity
  - Batch registration support

- **📆 Daily Attendance Tracking**
  - Quick mark attendance for all registered students
  - Date-stamped attendance records
  - Clear presence indicators: 'P' (Present) / 'A' (Absent)

- **🗂️ Dynamic Record Management**
  - Automatic creation of date columns in CSV files
  - Maintains complete attendance history
  - Easy export and backup of attendance data

- **✏️ Student Management**
  - Remove students from the attendance roster
  - Update student information
  - View complete attendance history per student

---

## 🛠️ Technical Stack

| Component | Technology |
|-----------|------------|
| **Language** | Python 3.x |
| **GUI Framework** | Tkinter |
| **Data Processing** | Pandas |
| **Data Storage** | CSV |
| **Date/Time** | datetime module |

---

## 📥 Installation

### Prerequisites

Ensure you have Python 3.x installed on your system. You can verify your Python installation by running:

```bash
python --version
# or
python3 --version
```

### Step-by-Step Installation

1. **Clone the repository**

```bash
git clone https://github.com/arpanpramanik2003/attendance-tracker.git
cd attendance-tracker
```

2. **Install required dependencies**

```bash
pip install pandas
# or
pip3 install pandas
```

> **Note:** Tkinter comes pre-installed with most Python distributions. If you encounter import errors, install it using:
> - **Ubuntu/Debian:** `sudo apt-get install python3-tk`
> - **Fedora:** `sudo dnf install python3-tkinter`
> - **macOS:** Included with Python installation
> - **Windows:** Included with Python installation

3. **Verify installation**

```bash
python attendance_tracker.py
```

---

## 🚀 Usage

### Quick Start

1. **Launch the application**

```bash
python attendance_tracker.py
```

2. **Login**
   - Enter your credentials at the login screen
   - Default credentials (if applicable) can be configured in the script

3. **Register Students**
   - Navigate to the student registration section
   - Enter student name and unique ID
   - Click "Register" to add the student

4. **Mark Attendance**
   - Select the date (defaults to current date)
   - Mark students as Present (P) or Absent (A)
   - Save attendance to update the CSV file

### Application Interface

![Attendance Tracker Interface](image_attendance_tracker.jpg)

*The intuitive interface allows quick navigation between student registration, attendance marking, and record management.*

### Workflow Example

```python
# Example workflow (conceptual)
1. Login → Authenticate user
2. Register Students → Add new entries to the system
3. Mark Attendance → Select date and mark P/A for each student
4. Save → Data written to attendance_records.csv
5. View History → Access historical attendance data
```

### CSV Output Format

The application generates CSV files with the following structure:

```csv
Name,UID,2024-01-15,2024-01-16,2024-01-17
John Doe,001,P,P,A
Jane Smith,002,P,A,P
Alex Johnson,003,A,P,P
```

**Column Descriptions:**
- `Name`: Student's full name
- `UID`: Unique identification number
- `Date columns`: Dynamically added columns showing attendance status (P/A)

---

## 📂 Code Structure

### Project Architecture

```
attendance-tracker/
│
├── attendance_tracker.py       # Main application file
├── README.md                   # Project documentation
├── image_attendance_tracker.jpg # Application screenshot
└── attendance_records.csv      # Generated attendance data (created on first use)
```

### Key Components

- **`attendance_tracker.py`**: Core application containing:
  - GUI components (Tkinter widgets)
  - Authentication logic
  - Student registration functions
  - Attendance marking functionality
  - CSV read/write operations
  - Data validation mechanisms

### Code Highlights

```python
# Key functionalities implemented:
- User authentication system
- Student CRUD operations
- Dynamic CSV column management
- Date-based attendance tracking
- Duplicate UID prevention
- Data persistence and retrieval
```

---

## 🔧 Configuration

### Customization Options

You can customize the application by modifying the following parameters in `attendance_tracker.py`:

- **Login credentials**: Update authentication details
- **CSV file path**: Change default save location
- **Date format**: Modify date representation
- **GUI theme**: Customize colors and layout

---

## ❓ Troubleshooting & FAQ

### Common Issues

**Q: I'm getting "ModuleNotFoundError: No module named 'pandas'"**

A: Install pandas using: `pip install pandas`

---

**Q: The GUI window is not appearing**

A: Ensure Tkinter is properly installed:
- Test with: `python -m tkinter`
- If a small window appears, Tkinter is working
- If not, reinstall Python with Tkinter support

---

**Q: My attendance data is not being saved**

A: Check the following:
- Verify write permissions in the application directory
- Ensure the CSV file is not open in another program
- Check for error messages in the console

---

**Q: Can I import existing student data?**

A: Yes, you can manually create or edit the CSV file with student names and UIDs before running the application.

---

**Q: How do I backup my attendance data?**

A: Simply copy the `attendance_records.csv` file to your preferred backup location. The CSV format ensures compatibility with Excel, Google Sheets, and other tools.

---

## 🤝 Contributing

We welcome contributions from the community! Here's how you can help:

### Ways to Contribute

- 🐛 Report bugs and issues
- 💡 Suggest new features or enhancements
- 📝 Improve documentation
- 🔧 Submit pull requests with fixes or features

### Contribution Guidelines

1. **Fork the repository**

```bash
git clone https://github.com/your-username/attendance-tracker.git
```

2. **Create a feature branch**

```bash
git checkout -b feature/your-feature-name
```

3. **Make your changes**
   - Write clean, documented code
   - Follow PEP 8 style guidelines
   - Test your changes thoroughly

4. **Commit your changes**

```bash
git commit -m "Add: Brief description of your changes"
```

5. **Push to your fork**

```bash
git push origin feature/your-feature-name
```

6. **Open a Pull Request**
   - Provide a clear description of your changes
   - Reference any related issues

### Code of Conduct

- Be respectful and constructive
- Welcome newcomers and help them learn
- Focus on collaboration and knowledge sharing

---

## 🗺️ Roadmap

### Upcoming Features

- [ ] **Database Integration** - SQLite/MySQL support for larger datasets
- [ ] **Export Options** - PDF and Excel export functionality
- [ ] **Advanced Analytics** - Attendance statistics and visualizations
- [ ] **Multi-user Support** - Role-based access control (Admin/Teacher/Viewer)
- [ ] **Cloud Sync** - Optional cloud storage integration
- [ ] **Mobile App** - Companion mobile application for Android/iOS
- [ ] **Email Notifications** - Automated absence alerts
- [ ] **Barcode/QR Scanner** - Quick student identification
- [ ] **Dark Mode** - UI theme options
- [ ] **Localization** - Multi-language support

### Version History

- **v1.0** - Initial release with core functionality
- Future versions will be documented here

---

## 📄 License

This project is licensed under the **MIT License** - see below for details:

```
MIT License

Copyright (c) 2024 Arpan Pramanik

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 📞 Support & Contact

- **Issues**: [GitHub Issues](https://github.com/arpanpramanik2003/attendance-tracker/issues)
- **Repository**: [GitHub Repository](https://github.com/arpanpramanik2003/attendance-tracker)
- **Author**: [Arpan Pramanik](https://github.com/arpanpramanik2003)

---

## 🙏 Acknowledgments

- Thanks to all contributors who help improve this project
- Built with Python and Tkinter
- Inspired by the need for simple, effective attendance management solutions

---

<div align="center">

**⭐ If you find this project useful, please consider giving it a star!**

Made with ❤️ by [Arpan Pramanik](https://github.com/arpanpramanik2003)

</div>
