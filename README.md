# 🏠 Mortgage Calculator

A modern, interactive mortgage calculator built with Streamlit that helps users calculate monthly payments, total interest, and visualize payment schedules over time.

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?logo=streamlit&logoColor=white)](https://streamlit.io/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 📋 Table of Contents

- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Installation](#-installation)
- [Usage](#-usage)
- [Project Structure](#-project-structure)
- [How It Works](#-how-it-works)
- [Contributing](#-contributing)
- [License](#-license)

## ✨ Features

- 💰 **Real-time Calculations**: Instantly calculates monthly payments as you adjust inputs
- 📊 **Interactive Visualization**: Dynamic line charts showing remaining balance over time
- 📅 **Flexible Time Views**: Switch between monthly and yearly payment schedules
- 💳 **Comprehensive Metrics**: Displays monthly payments, total repayments, and total interest
- 📈 **Payment Schedule**: Detailed breakdown of principal vs. interest payments
- 🎨 **Clean UI**: Intuitive and user-friendly interface built with Streamlit
- ⚡ **Fast Performance**: Lightweight application with instant calculations

## 🛠️ Tech Stack

| Technology | Purpose | Repository |
|------------|---------|------------|
| ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white) | Core Programming Language | [python.org](https://www.python.org/) |
| ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white) | Web Framework & UI | [github.com/streamlit/streamlit](https://github.com/streamlit/streamlit) |
| ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white) | Data Manipulation & Analysis | [github.com/pandas-dev/pandas](https://github.com/pandas-dev/pandas) |

### Key Libraries

- **[Streamlit](https://streamlit.io/)** - Framework for building interactive web applications
- **[Pandas](https://pandas.pydata.org/)** - Data structures and analysis tools for payment schedules
- **Math** (Built-in) - Mathematical calculations for loan amortization

## 📦 Installation

### Prerequisites

- Python 3.8 or higher
- pip (Python package manager)

### Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/jblnco-ing/mortgage_calculator_streamlit.git
   cd mortgage_calculator_streamlit
   ```

2. **Create a virtual environment** (recommended)
   ```bash
   # Windows
   python -m venv venv
   venv\Scripts\activate

   # macOS/Linux
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

## 🚀 Usage

1. **Run the application**
   ```bash
   streamlit run app.py
   ```

2. **Access the application**
   - The app will automatically open in your default browser
   - Or navigate to `http://localhost:8501`

3. **Use the calculator**
   - Enter the home value
   - Input your deposit amount
   - Set the interest rate (annual percentage)
   - Choose the loan term in years
   - View real-time calculations and payment schedule

## 📁 Project Structure

```
mortgage_calculator_streamlit/
├── app.py              # Main application file
├── requirements.txt    # Python dependencies
├── .gitignore         # Git ignore rules
├── pyrightconfig.json # Python type checking configuration
└── README.md          # Project documentation
```

## 🧮 How It Works

The calculator uses the standard amortization formula to compute monthly payments:

```
M = P × [r(1 + r)^n] / [(1 + r)^n - 1]
```

Where:
- **M** = Monthly payment
- **P** = Principal loan amount (Home Value - Deposit)
- **r** = Monthly interest rate (Annual Rate / 12 / 100)
- **n** = Total number of payments (Loan Term × 12)

### Calculation Process

1. **Input Processing**: Collects user inputs for home value, deposit, interest rate, and loan term
2. **Payment Calculation**: Applies the amortization formula to calculate monthly payments
3. **Schedule Generation**: Creates a detailed payment schedule showing:
   - Principal payment per period
   - Interest payment per period
   - Remaining balance after each payment
4. **Visualization**: Generates interactive charts for easy understanding of payment progression

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Juan Blanco**

- GitHub: [@jblnco-ing](https://github.com/jblnco-ing)

## 🙏 Acknowledgments

- Built with [Streamlit](https://streamlit.io/)
- Data manipulation powered by [Pandas](https://pandas.pydata.org/)
- Inspired by the need for simple, accessible financial calculators

---

⭐ If you find this project useful, please consider giving it a star!
