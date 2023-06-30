# Web Scraping and Text Retrieval

This repository contains a Python script for web scraping and text retrieval from a given website. The script utilizes the `requests`, `beautifulsoup4`, `urllib`, `pathlib`, and `google.colab` libraries to retrieve and save text content from web pages.

## Getting Started

To get started with this script, follow the instructions below.

### Prerequisites

- Python 3.6 or higher
- Install the required libraries using the following command:
  ```bash
  pip install requests beautifulsoup4 google-colab
  ```

### Usage

1. Clone this repository to your local machine or download the script file directly.
2. Open the script file (`scrape_text.py`) in a text editor of your choice.

### Configuration

1. Mount Google Drive by running the following command:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```
   This step is required to save the retrieved text files to Google Drive.

2. Set the `url` variable to the URL of the main page you want to start scraping from:
   ```python
   url = 'https://quod.lib.umich.edu/c/cme/browse.html'
   ```

### Running the Script

To run the script, execute the following command:
```bash
python scrape_text.py
```

The script will start following the links from the main page specified in the `url` variable. It will recursively retrieve text content from nested links and save them as `.txt` files in the specified Google Drive directory.

### Displaying All Fonts

To display all the available fonts, you can modify the script as follows:

1. Import the necessary libraries:
   ```python
   import matplotlib.pyplot as plt
   import matplotlib.font_manager as fm
   ```

2. Add the following code snippet after the line `drive.mount('/content/drive')`:
   ```python
   # Get a list of all available fonts
   all_fonts = fm.findSystemFonts()

   # Display each font name
   for font_path in all_fonts:
       font_name = fm.get_font(font_path).family_name
       print(font_name)
   ```

   This code will retrieve a list of all available fonts on your system and print their names.

## Contributing

Contributions to this repository are welcome. If you find any issues or have suggestions for improvements, please create a pull request or open an issue.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- The developers of the websites being scraped for providing the text in the public domain so that they can be used freely for any purpose.
