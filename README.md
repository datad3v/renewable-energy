# Renewable Energy Grid Balancing Simulation

## Overview

This project simulates the integration of renewable energy sources (solar and wind) into the power grid while implementing a battery storage system and demand response mechanism to balance fluctuations. The goal is to ensure stable energy distribution despite varying power generation and consumption patterns.

## Features

- **Solar & Wind Power Generation**: Uses real-world data to model renewable energy contributions.
- **Electricity Demand Simulation**: Models power consumption based on real-time demand data.
- **Battery Storage System**: Stores excess energy and discharges when demand exceeds generation.
- **Demand Response Mechanism**: Adjusts demand dynamically to balance the grid.
- **Visualization**: Graphs show energy generation, demand, and grid balance over time.

## Tech Stack

- **Python** (Backend and Data Processing)
  - Pandas: Data handling
  - NumPy: Numerical computations
  - Matplotlib: Data visualization
- **Data Sources**
  - Open Power System Data
  - NREL Solar/Wind Resource Data
  - NYISO or PJM Hourly Load Data

## Installation & Setup

### Prerequisites

Ensure you have Python installed along with the required libraries:

```bash
pip install pandas numpy matplotlib
```

### Running the Simulation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/grid-balancing-simulation.git
   ```
2. Navigate to the project directory:
   ```bash
   cd grid-balancing-simulation
   ```
3. Place your dataset files (`solar_generation.csv`, `wind_generation.csv`, `electricity_demand.csv`) in the `data/` folder.
4. Run the main script:
   ```bash
   python simulate_grid.py
   ```

## How It Works

1. **Load Data**: Reads solar, wind, and demand datasets.
2. **Calculate Total Generation**: Aggregates renewable energy production.
3. **Balance the Grid**:
   - If excess energy is available, store it in the battery.
   - If demand exceeds generation, discharge from the battery.
   - Adjust demand where possible through demand response mechanisms.
4. **Visualization**: Generates a plot showing energy balance over time.

## Example Output

- A time-series graph showing energy surplus/deficit and battery charge levels.

## Future Enhancements

- Add efficiency constraints to battery storage.
- Implement dynamic pricing to model economic impacts.
- Develop a Streamlit-based UI for interactive analysis.

## Contribution

Feel free to contribute by submitting issues or pull requests!

## License

This project is licensed under the MIT License.

---

### Contact

For questions or suggestions, reach out via GitHub Issues or email at [datad3v].

