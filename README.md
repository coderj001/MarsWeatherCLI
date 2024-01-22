## Python Typer CLI App for Mars Weather Data

This readme file guides you through the Python Typer CLI application designed to fetch and display weather data from Mars, utilizing data provided by NASA.

### Purpose

This CLI tool leverages the power of Python's Typer library to build a user-friendly interface for accessing real-time Martian weather information. It eliminates the need for web browsing, offering a convenient way to retrieve weather data for quick checks or automation purposes.

### Features

* Fetch current weather conditions (temperature, pressure, wind speed, etc.) for various Martian locations, including Curiosity rover landing site and InSight lander location.
* Retrieve weather data for a specified date range.
* Display weather data in a clear and concise format.
* Offer user-friendly flags for customizing output and behavior.

### Installation

1. **Requirements:** Ensure Python 3.7+ and `typer` package are installed.
2. **Clone the repository:** `git clone https://github.com/your-username/mars-weather-cli`
3. **Install dependencies:** `pip install -r requirements.txt`

### Usage

Run the script using the following command:

```bash
python main.py [OPTIONS] <LOCATION> [START_DATE] [END_DATE]
```

**Options:**

* `-h, --help`: Display help message.
* `-v, --version`: Show program version.
* `-i, --image`: Include an image of the specified location (Curiosity or InSight) in the output.

**Examples:**

* Get current weather at Curiosity rover landing site:

```bash
python main.py curiosity
```

* View weather data from InSight lander for the past week:

```bash
python main.py insight 2024-01-15 2024-01-22
```

* Retrieve weather data for Curiosity rover from January 1st to 10th, 2024, and include an image of the landing site:

```bash
python main.py curiosity 2024-01-01 2024-01-10 -i
```

### Contributing

Feel free to contribute to this project by:

* Reporting bugs or suggesting improvements.
* Adding support for additional Martian weather data sources.
* Enhancing the CLI interface and user experience.

For contribution guidelines, please refer to the CONTRIBUTING.md file.

### Disclaimer

This application relies on NASA's Mars weather APIs for data retrieval. While efforts are made to ensure accuracy, the provided weather information may not always be 100% precise. Be mindful of this when making critical decisions based on the displayed data.

### Conclusion

We hope this CLI application simplifies your access to weather data on Mars. Use it for quick weather updates, automate weather checks in scripts, or even build upon it to create your own customized Martian weather tools. Enjoy exploring the Red Planet's weather patterns!
