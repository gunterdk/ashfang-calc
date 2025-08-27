# Ashfang Damage Simulator

A web-based damage calculator for the Ashfang boss fight that calculates net damage based on blazes killed and boss healing mechanics.

## Features

- **Interactive Slider**: Adjust the number of blazes killed (0-12) to see how it affects damage calculations
- **Real-time Calculations**: Instantly updates damage dealt, healing received, and net damage
- **Attempt Estimation**: Calculates how many attempts are needed to defeat the boss
- **Dark/Light Mode**: Toggle between color themes for comfortable viewing
- **Detailed Breakdown**: Expandable section showing the complete calculation steps
- **Responsive Design**: Works on both desktop and mobile devices

## How It Works

The simulator models a boss fight with the following mechanics:
- Boss HP: 50,000,000
- Damage per blaze orb: 2,000,000
- Healing per remaining blaze: 500,000
- Total blazes: 12

### Calculation Formula
Damage Dealt = Blazes Killed × 2,000,000
Healing Received = (12 - Blazes Killed) × 500,000
Net Damage = Damage Dealt - Healing Received
Attempts Needed = ceil(50,000,000 / Net Damage)
## Usage

1. Use the slider to select how many blazes you've killed (0-12)
2. View the net damage result in the main display
3. Expand "Calculation Details" to see the complete breakdown
4. See how many attempts would be needed to defeat the boss
5. Toggle dark/light mode using the button in the bottom-right corner

## Technical Details

- Built with vanilla HTML, CSS, and JavaScript
- Uses Font Awesome for icons
- Responsive design with CSS Flexbox
- CSS animations for value changes
- No external dependencies beyond the Font Awesome CDN

## Browser Compatibility

Works in all modern browsers that support:
- CSS Flexbox
- CSS Variables
- ES6 JavaScript features

## License

Open source - feel free to use and modify as needed.
