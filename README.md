# BMI Calculator Web Application

A simple and elegant Body Mass Index (BMI) calculator built with Node.js, Express, and vanilla JavaScript.

##  Features

- **User-friendly Interface**: Clean and responsive design with color-coded results
- **BMI Calculation**: Accurate BMI calculation using the standard formula
- **Input Validation**: Both client-side and server-side validation
- **Category Classification**: Automatically categorizes BMI into Underweight, Normal, Overweight, or Obese
- **Health Advice**: Provides basic health recommendations based on BMI category
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices

##  Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm (Node Package Manager)

### Installation

1. **Clone the repository:**
```bash
git clone <your-repository-url>
cd bmi-calculator
```

2. **Install dependencies:**
```bash
npm install
```

3. **Run the application:**
```bash
npm start
```

4. **Open your browser and navigate to:**
```
http://localhost:3000
```

##  Project Structure

```
bmi-calculator/
├── node_modules/          # Dependencies
├── public/                # Static files
│   ├── css/
│   │   └── style.css     # Application styling
│   └── js/
│       └── validation.js  # Client-side validation
├── views/
│   └── index.html        # Main HTML page
├── server.js             # Express server
├── package.json          # Project configuration
├── .gitignore           # Git ignore rules
└── README.md            # Documentation
```

##  Technologies Used

- **Backend**: Node.js, Express.js
- **Frontend**: HTML5, CSS3, JavaScript
- **Middleware**: body-parser

##  BMI Categories

| Category | BMI Range |
|----------|-----------|
| Underweight | BMI < 18.5 |
| Normal weight | 18.5 ≤ BMI < 24.9 |
| Overweight | 25 ≤ BMI < 29.9 |
| Obese | BMI ≥ 30 |

##  Color Coding

- **Blue**: Underweight
- **Green**: Normal weight
- **Yellow**: Overweight
- **Red**: Obese

##  Formula

```
BMI = weight (kg) / height² (m²)
```

##  Validation

The application includes comprehensive validation:

- **Client-side**: Real-time validation using JavaScript
- **Server-side**: Backend validation in Express routes
- Checks for empty fields
- Validates positive numbers
- Ensures reasonable value ranges

##  API Endpoints

### GET `/`
Returns the main HTML form for BMI input.

### POST `/calculate-bmi`
Calculates BMI and returns the result page.

**Request Body:**
```json
{
  "weight": "70",
  "height": "1.75"
}
```

**Response:** HTML page with calculated BMI and category

##  Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

##  License

This project is licensed under the MIT License.

##  Author

Your Name

##  Acknowledgments

- Assignment from [Your University/Course Name]
- BMI calculation standards from WHO guidelines
