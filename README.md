<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      margin: 0;
      padding: 20px;
    }

    h1 {
      font-family: 'Times New Roman', Times, serif;
      font-size: 28px;
      margin-top: 0;
    }

    h2 {
      font-family: 'Arial Black', sans-serif;
      font-size: 22px;
    }

    p {
      font-family: 'Courier New', monospace;
      margin-bottom: 10px;
    }

    code {
      font-family: Consolas, Monaco, 'Andale Mono', monospace;
      background-color: #f1f1f1;
      padding: 3px;
      border-radius: 3px;
    }

    pre {
      font-family: 'Lucida Console', Monaco, monospace;
      background-color: #f1f1f1;
      padding: 10px;
      border-radius: 5px;
      overflow-x: auto;
    }

    .important {
      font-weight: bold;
      color: #c00;
    }

    .highlight {
      background-color: yellow;
    }

    .container {
      max-width: 800px;
      margin: 0 auto;
    }
  </style>
</head>

<body>
  <div class="container">
    <h1>Web Scraping and Text Retrieval</h1>

    <p>This repository contains a Python script for web scraping and text retrieval from a given website. The script
      utilizes the <code>requests</code>, <code>beautifulsoup4</code>, <code>urllib</code>, <code>pathlib</code>, and
      <code>google.colab</code> libraries to retrieve and save text content from web pages.</p>

    <h2>Getting Started</h2>

    <p>To get started with this script, follow the instructions below.</p>

    <h3>Prerequisites</h3>

    <ul>
      <li>Python 3.6 or higher</li>
      <li>Install the required libraries using the following command:</li>
    </ul>

    <pre><code>pip install requests beautifulsoup4 google-colab</code></pre>

    <h3>Usage</h3>

    <ol>
      <li>Clone this repository to your local machine or download the script file directly.</li>
      <li>Open the script file (<code>scrape_text.py</code>) in a text editor of your choice.</li>
    </ol>

    <h3>Configuration</h3>

    <ol>
      <li>Mount Google Drive by running the following command:</li>
    </ol>

    <pre><code>from google.colab import drive
drive.mount('/content/drive')</code></pre>

    <p>This step is required to save the retrieved text files to Google Drive.</p>

    <ol start="2">
      <li>Set the <code>url</code> variable to the URL of the main page you want to start scraping from:</li>
    </ol>

    <pre><code>url = 'https://quod.lib.umich.edu/c/cme/browse.html'</code></pre>

    <h3>Running the Script</h3>

    <p>To run the script, execute the following command:</p>

    <pre><code>python scrape_text.py</code></pre>

    <p>The script will start following the links from the main page specified in the <code>url</code> variable. It
      will recursively retrieve text content from nested links and save them as <code>.txt</code> files in the specified
      Google Drive directory.</p>

    <h2>Contributing</h2>

    <p>Contributions to this repository are welcome. If you find any issues or have suggestions for improvements, please
      create a pull request or open an issue.</p>

    <h2>License</h2>

    <p>This project is licensed under the <a href="LICENSE">MIT License</a>.</p>

    <h2>Acknowledgments</h2>

    <ul>
      <li>The <code>requests</code>, <code>beautifulsoup4</code>, <code>urllib</code>, <code>pathlib</code>, and
        <code>google.colab</code> libraries for their functionalities used in this script.</li>
      <li>The developers of the websites being scraped for providing valuable content.</li>
    </ul>

    <p>Feel free to customize this README file to suit your project's needs.</p>
  </div>
</body>

</html>
