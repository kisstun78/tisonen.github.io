# Engine Compression Calculator

A web application for calculating compression ratio and dynamic compression ratio of a single-cylinder engine using Vue 3.

## Features

- Calculate static compression ratio based on:
  - Bore diameter
  - Stroke length
  - Clearance volume
  - Deck height
  - Head gasket thickness
  - Head gasket bore diameter
  - Piston dome/dish volume

- Calculate dynamic compression ratio based on:
  - All static compression parameters
  - Connecting rod length
  - Cam duration
  - Lobe separation angle
  - Intake valve opening timing
  - Exhaust valve closing timing

- Display additional calculated values:
  - Swept volume
  - Total cylinder volume
  - Gasket volume
  - Deck volume
  - Effective clearance volume
  - Intake closing point

## Usage

1. Open `index.html` in a web browser
2. Enter the engine parameters in the input fields
3. The compression ratios will be calculated automatically

## Technical Details

- Built with Vue 3 Composition API
- Uses CDN-hosted Vue.js (no build step required)
- Styled with Bootstrap 5
- Performs real-time calculations as values change

## Formulas Used

### Static Compression Ratio
```
CR = (Swept Volume + Clearance Volume) / Clearance Volume
```

### Dynamic Compression Ratio
```
DCR = (Swept Volume from IVC + Clearance Volume) / Clearance Volume
```
Where IVC is the Intake Valve Closing point.

## License

MIT