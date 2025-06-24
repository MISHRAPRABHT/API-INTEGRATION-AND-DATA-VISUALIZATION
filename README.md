COMPANY: CODETECH IT SOLUTIONS
NAME: PRABHAT KUMAR MISHRA 
INTERN ID: CT06DM568
DOMAIN: PYTHON DEVELOPEMENT
DURATION: 6 WEEKS
MENTOR: NEELA SANTOSH
DESCRIPTION-
Project Overview
This project develops a Python script to fetch a 5-day hourly weather forecast for London using the Open-Meteo API. The script processes the data into a structured format, generates visualizations to analyze temperature trends, weather condition frequencies, and temperature-humidity relationships, and saves a text summary of the current weather. The goal is to provide clear, actionable insights into weather patterns through data processing and visualization.
Progress Summary
The script, executed on Python 3.11.9 (Windows 64-bit), has been successfully reviewed. Below is a detailed status of each component:
Environment Setup:
Status: Completed

Details: The script imports required libraries (requests, pandas, matplotlib, seaborn), confirming a properly configured environment.

Observation: No compatibility issues with Python or libraries were noted.

Data Acquisition:
Status: Completed

Details: The script retrieves hourly weather data (temperature, humidity, precipitation probability, weather codes) for London (latitude: 51.5074, longitude: -0.1278) via the Open-Meteo API for a 5-day forecast.

Observation: The get_forecast function handles API errors (status code checks), ensuring robust data fetching. No connectivity issues were observed during execution.

Data Processing:
Status: Completed

Details: The API’s JSON response is converted into a pandas DataFrame with columns for time, temperature, humidity, precipitation probability, and weather codes. Weather codes are mapped to descriptive labels (e.g., “Clear,” “Light Rain”) using a dictionary.

Observation: The weather code mapping covers a subset of codes (0, 1, 2, 3, 51, 61, 63, 80), with unmapped codes labeled “Other.” This may limit granularity for rare conditions. Timestamps are correctly parsed as datetime objects.

Data Visualization:
Status: Completed

Details: Three visualizations are generated and saved as PNG files:
Temperature over Time (temperature_forecast.png): A line plot with markers showing temperature trends.

Weather Conditions Frequency (weather_conditions.png): A bar plot of weather type counts.

Temperature vs Humidity (temp_vs_humidity.png): A scatter plot with weather-based coloring and precipitation probability-based sizing.

Observation: Visualizations use seaborn for a professional look, with clear titles, labels, and rotated x-axis ticks. No plotting errors were noted.

Data Output:
Status: Completed

Details: A text file (current_weather.txt) saves a summary of the first hourly data point’s temperature, weather condition, and humidity.

Observation: The “current” weather is taken from the first data point, which may not align precisely with the actual current time.

Key Achievements
Successfully fetched and processed 5-day weather forecast data from the Open-Meteo API.

Created three high-quality visualizations to analyze temperature, weather frequency, and temperature-humidity relationships.

Generated a text summary of the current weather for quick reference.

Implemented basic error handling for API requests.

Applied consistent seaborn styling for professional visualizations.

Potential Improvements
Weather Code Mapping: Expand the weather_map dictionary to include more Open-Meteo API codes (e.g., snow, fog) for better condition coverage.

Current Weather Selection: Filter the DataFrame for the timestamp closest to the current time instead of using the first data point.

Visualization Enhancements: Add annotations to the temperature plot and a legend for precipitation probability in the scatter plot.

Error Handling: Include checks for missing API fields or network timeouts.

Output Flexibility: Allow users to specify output directories for files and export the DataFrame as a CSV.

Next Steps
Testing: Validate the script with different locations and cross-reference weather codes with API documentation.

Enhancements: Implement expanded weather code mapping and refined current weather logic within 1-2 days.

Configuration: Add user-configurable parameters (e.g., location, forecast days) via command-line arguments in 3-5 days.

Documentation: Create a README with usage instructions in 7 days.

Issues Encountered
No errors were reported, as indicated by the [DEBUG ON] and [DEBUG OFF] markers. Potential issues, such as unmapped weather codes or API rate limits, should be monitored in future use.
Timeline
Completed: Data fetching, processing, visualization, and text output.

Next 1-2 Days: Address weather code mapping and current weather selection.

Next 3-5 Days: Add configurable parameters.

Next 7 Days: Finalize documentation.

Conclusion
The project is fully functional, delivering weather data and insightful visualizations for London. The script is well-organized, with opportunities for minor enhancements to improve accuracy and usability. It is on track for completion, with potential for advanced features like user inputs or a GUI. Please advise on priority areas or additional requirements.


OUTPUT
![Image](https://github.com/user-attachments/assets/9b89b2b4-0faa-4568-97c6-e0162d9044cf)
![Image](https://github.com/user-attachments/assets/a83ccb0d-aaed-463a-8e8b-e73157d9c302)
![Image](https://github.com/user-attachments/assets/fb5c9d70-9b9b-421b-859c-7d783beaf28a)
![Image](https://github.com/user-attachments/assets/ec65989c-0d78-4d2c-ad26-620e1cb4e022)


