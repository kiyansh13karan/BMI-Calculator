# BMI Calculator 🏃‍♀️

A beautiful, responsive Body Mass Index (BMI) calculator with a serene yoga-themed interface. This web application allows users to calculate their BMI quickly and provides instant feedback on their health status.

![BMI Calculator Interface](![Image](https://github.com/user-attachments/assets/9da9f8e2-7f7c-4899-bab2-080b5ac579b8))

## 🌟 Features

- **Clean & Modern UI**: Glassmorphism design with a calming yoga background
- **Responsive Design**: Works seamlessly across different screen sizes
- **Real-time Validation**: Instant input validation with helpful error messages
- **BMI Categories**: Displays weight categories (Underweight, Normal, Overweight)
- **Precise Calculations**: BMI calculated to 2 decimal places for accuracy
- **User-friendly Interface**: Simple form with clear labels and intuitive design

## 🛠️ Technologies Used

- **HTML5**: Semantic markup structure
- **CSS3**: Modern styling with backdrop-filter effects and flexbox layout
- **JavaScript (ES6)**: Form handling, calculations, and DOM manipulation
- **Responsive Design**: Viewport-based units (vw, vh) for adaptability

## 📊 BMI Categories

The calculator uses the following BMI ranges:

| Category | BMI Range |
|----------|-----------|
| **Underweight** | Less than 18.6 |
| **Normal Range** | 18.6 - 24.9 |
| **Overweight** | Greater than 24.9 |

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- Basic understanding of HTML/CSS/JavaScript (for modifications)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/bmi-calculator.git
   cd bmi-calculator
   ```

2. **Open the project**
   ```bash
   # Simply open index.html in your browser
   open index.html
   ```
   
   Or use a local server:
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Node.js (if you have live-server installed)
   npx live-server
   ```

3. **Access the application**
   - Open your browser and navigate to `http://localhost:8000` (if using a server)
   - Or directly open the `index.html` file in your browser

## 📁 Project Structure

```
bmi-calculator/
│
├── index.html          # Main HTML structure
├── style.css           # Styling and layout
├── script.js           # JavaScript functionality
├── yoga.jpg            # Background image
├── screenshot.png      # Interface screenshot
└── README.md           # Project documentation
```

## 🎨 Design Features

- **Glassmorphism Effect**: Semi-transparent container with backdrop blur
- **Yoga Theme**: Peaceful background promoting wellness
- **Typography**: Clean, readable fonts with proper contrast
- **Color Scheme**: Soft, calming colors that enhance user experience
- **Responsive Layout**: Adapts to different screen sizes

## 🔧 Code Highlights

### BMI Calculation Formula
```javascript
const bmi = (weight / ((height * height) / 10000)).toFixed(2);
```

### Input Validation
- Checks for empty fields
- Validates numeric input
- Prevents negative values
- Provides user-friendly error messages

### Event Handling
- Form submission prevention
- Real-time calculation
- Dynamic result display

## 🐛 Known Issues

1. **BMI Calculation Bug**: There's currently a bug in the BMI formula in `script.js` line 14:
   ```javascript
   // Current (incorrect):
   const bmi = (weight / ((height *
