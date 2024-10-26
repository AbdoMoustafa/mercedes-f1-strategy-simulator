# Mercedes F1 Race Strategy Predictor & Competitive Analysis

This project is a Mercedes F1 Race Strategy Predictor that models race strategies for Lewis Hamilton and compares them against Max Verstappen's strategy, as well as analysing sector times and where Hamilton is losing time. It simulates race scenarios with a focus on tire compound degradation, pit stops, and adaptability across different track conditions. Although the example provided focuses on Bahrain, the model is adaptable to various circuits and weather conditions, including rain (intermediate and wet tires).

### Project Highlights

- **Competitive Analysis**: Simulates various race strategies for Bahrain, concluding that Hamilton's optimal approach is a conservative single-stop strategy (Medium → Hard), while Verstappen's simulated best strategy is a more aggressive two-stop (Medium → Soft → Hard). This difference reflects Red Bull's current pace advantage in the new regulatory era, allowing for a more assertive tire management approach.
- **Dynamic Degradation Modeling**: Models tire degradation by compound (including intermediate and wet tires), factoring in temperature variability and random fluctuations.
- **Adaptability Across Tracks**: Designed for different tracks and conditions, allowing comparisons between circuits like Bahrain and Silverstone.
- **Sector Time Analysis**: Compares and visualizes sector times between Hamilton and Verstappen, identifying specific areas where Hamilton may be losing time. This analysis provides insights into potential areas for improvement in driving technique or car setup.

### Features

1. **Tire Compound Modeling**: Supports all F1 compounds—Soft, Medium, Hard, Intermediate, and Wet—simulating degradation and performance changes based on lap count and temperature.
2. **Race Strategy Prediction**: Uses multi-stop simulations, including one- and two-stop strategies, to optimize lap times and minimize pit-stop loss.
3. **Simulated Real-Time Weather Variation**: Adds an array to vary track temperature across the race, simulating real-time data changes in place of live data access.
4. **Visual Insights**: Cumulative degradation plots, compound usage charts, and comparative lap analysis highlight strategic differences between Hamilton and Verstappen.

### Limitations

The model is subject to certain constraints:

1. **API Constraints**: Limited real-time weather and competitor data restrict live adaptability.
2. **Static Pit Stop Times**: Assumes consistent pit stop times, which may vary due to unforeseen race conditions.
3. **Simplified Track and Weather Model**: Weather is modeled with basic parameters, which may not fully capture real-world complexity.
4. **No Fuel Load Impact**: Currently excludes fuel load as a variable due to lack of detailed data.

### Libraries and Tools

- Data Manipulation: pandas, numpy
- Machine Learning: scikit-learn
- Visualization: matplotlib
- Statistical Analysis: scipy
- F1 Data Access: fastf1

### Installation

1. Clone the repository:

   ```
   git clone <repository-url>
   ```

2. Install dependencies:
   ```
   pip install numpy pandas matplotlib scipy scikit-learn fastf1
   ```

### Usage

1. **Run the Notebook**: Open `simulator.ipynb` in Jupyter Notebook to view code, run simulations, and generate insights.
2. **Customizable Inputs**: Modify inputs like track, drivers, track temperature etc. to simulate various track conditions.
3. **Visualize Results**: Generate degradation plots, strategy comparisons, and compound usage charts to assess race strategies.

### Future Enhancements

1. **Advanced Real-Time Adjustments**: Add predictive modeling to adapt strategies dynamically based on simulated race events.
2. **Expanded Weather and Condition Models**: Integrate a more complex weather and track evolution model to improve accuracy in varied conditions.
