# Madden Ratings Scraper

This script downloads Madden ratings data for a given range of years from `https://maddenratings.weebly.com/`. It stores the data as CSV files in a directory named `madden_data`.

## Installation

1. Clone the repository and navigate to its directory.

2. Create a Python virtual environment:

    ```bash
    python3 -m venv venv
    ```

3. Activate the virtual environment:

    On Unix or MacOS, run:
    
    ```bash
    source venv/bin/activate
    ```
    
    On Windows, run:
    
    ```cmd
    venv\Scripts\activate.bat
    ```

4. Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

## Usage

To run the script, use the following command, providing the years you want to download data for:

```bash
python madden_ratings_scraper.py --from 05 --to 20
```

Without any arguments, the script will default to downloading data for all years from 02 to the current year + 1:

```bash
python madden_ratings_scraper.py
```

To consolidate your downloaded data into a single, unified .csv file, you can utilize the `combine_madden_ratings.py` script. Execute this script by opening your terminal and entering the following command:

```bash
python combine_madden_ratings.py
```

Upon the successful execution of the script, the resultant file will be stored in the `processed_data` directory. 

## License

This project is open-source and available to everyone under the [MIT License](https://opensource.org/licenses/MIT).

## Contribution

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## Acknowledgments

This project uses data from the [Madden Ratings](https://maddenratings.weebly.com/) website.

## Disclaimer

This script is for educational purposes only. Please respect the terms of use and privacy policies of any websites you scrape.
