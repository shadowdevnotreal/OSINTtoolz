![2024-03-05_01-42-08](https://github.com/shadowdevnotreal/OSINTtoolz/assets/43219706/cf59a8ae-dbe2-4c3c-b55a-cdf11ef91244)

## Support FOSS future development - Simping for donations here 👇

<a href="https://www.buymeacoffee.com/notarealdev">
    <img src="https://img.buymeacoffee.com/button-api/?text=Buy me a cat&emoji=🐈&slug=notarealdev&button_colour=9123cd&font_colour=ffffff&font_family=Bree&outline_colour=ffffff&coffee_colour=FFDD00" />
</a>

---
***SHOUT OUT TO https://github.com/cyberpunkOS/CyberPunkOS for the inspiration for this code***

# OSINT Tools Suite

This repository contains a collection of Open Source Intelligence (OSINT) tools designed to aid in the gathering of publicly available information from various sources on the internet. Among these tools is a Python script for searching news articles across multiple RSS feeds based on a keyword.

## News Search Script

The news search script allows users to search for news articles containing specific keywords across various RSS feeds. It dynamically installs necessary dependencies, performs the search, and saves the results in a structured format.

### Features

- **Keyword Search**: Search multiple news RSS feeds for articles containing a specific keyword.
- **Dynamic Dependency Installation**: Automatically checks for and installs required Python packages.
- **Customizable RSS Feed List**: Easily add or remove RSS feeds from the search list.
- **Results Storage**: Saves search results in a timestamped text file for easy reference.

### Installation

Before running the script, ensure you have Python 3 and pip installed on your system. The script has been tested on Linux, macOS, and Windows.

1. **Clone the repository**:
   ```bash
   git clone https://github.com/shadowdevnotreal/OSINTtoolz.git
   ```
2. **Navigate to the script's directory**:
   ```bash
   cd OSINTtoolz
   ```

### Usage

To use the news search script, simply run it from the command line with a keyword as its argument. The script will handle dependency installation (if needed) and proceed with the search.

```bash
python newsfeed.py "keyword"
```

Replace `"keyword"` with the term you wish to search for.

### Adding RSS Feeds

To add more RSS feeds to the script, open `search_news.py` in a text editor and locate the `feeds` list. Add your new feed URLs to the list, enclosed in quotes. You can use either single (`'`) or double (`"`) quotes for consistency:

```python
feeds = [
    'http://www.example.com/rss',
    "http://www.anotherexample.com/rss",
    # Add more feeds as needed
]
```

### FAQ

**Q: Do I need to install any packages before running the script?**  
A: No, the script will automatically check for and install the required `feedparser` package upon execution.

**Q: Can I run this script on any operating system?**  
A: Yes, the script is designed to be platform-agnostic, as long as you have Python 3 and pip installed.

**Q: How can I contribute to this project?**  
A: Contributions are welcome! Please feel free to fork the repository, make your changes, and submit a pull request.

---


# Photon Scanner Tool

The Photon scanner is a powerful OSINT (Open Source Intelligence) tool designed for website scanning and cloning. It allows users to quickly gather a wealth of information from a specified website, including the site's files, directories, and external links. This guide will help you set up and use the Photon scanner tool stored in this repository.

## Features

- **Website Scanning**: Extracts and reports detailed information about the target website's structure and contents.
- **Website Cloning**: Downloads a copy of the website for offline analysis.
- **Flexible Output**: Saves scan and clone results in a user-specified directory.

## Installation

Before using the Photon scanner, ensure you have `git`, `Python 3`, and `pip` installed on your system.

### Step 1: Clone the Repository

First, clone this repository to your local machine. Open a terminal and run:

```bash
git clone https://github.com/shadowdevnotreal/OSINTtoolz.git
cd OSINTtoolz
```

### Step 2: Install Photon

The script automatically checks if Photon is installed in the `OSINTtoolz` directory within your home folder. If it's not found, the script will clone Photon from its GitHub repository.

## Usage

Navigate to the script's directory, then run the script from the terminal:

```bash
./photon2.sh
```

Follow the on-screen prompts to select your desired operation:

1. **Scan website**: Enter the URL of the website you wish to scan.
2. **Clone website**: Enter the URL of the website you wish to clone for offline access.
3. **Return to main menu**: Exit or perform another operation.

### Adding More Functions

You can modify the script to add more functionalities of Photon by editing the `photon2.sh` script and following the Photon documentation for additional command-line arguments.

## FAQ

**Q: What do I need to run the Photon scanner?**  
A: You need `git`, `Python 3`, and `pip` installed. The script takes care of installing Photon itself.

**Q: How can I contribute to this project?**  
A: Contributions are welcome! Feel free to fork the repository, make improvements, and submit a pull request.

**Q: Where are the scan results saved?**  
A: Results are saved in the `OSINTTools/results` directory within your home folder. Each operation's output is stored in a separate folder named after the target website.

---


# Sherlock Scanner Tool

The Sherlock scanner tool is designed for discovering user accounts across various social platforms given a username. This powerful OSINT tool can help in identifying the online presence of a specific username across multiple platforms, making it invaluable for researchers, investigative journalists, and anyone interested in digital footprint analysis.

## Features

- **Basic Search**: Quickly checks the presence of a username across popular social networks.
- **Multi-User Search**: Allows searching for multiple usernames in one go.
- **Verbose Mode Search**: Provides detailed search results, including HTTP response codes.
- **Search on All Platforms**: Extends the search across all supported platforms for thorough analysis.

## Installation

Before you begin, ensure you have `git`, `Python 3`, and `pip` installed on your system.

### Step 1: Clone the Repository

First, clone this repository to your local machine. Open a terminal and execute:

```bash
git clone https://github.com/shadowdevnotreal/OSINTtoolz.git
cd OSINTtoolz
```

### Step 2: Install Sherlock

If Sherlock is not already installed in the `OSINTtoolz/sherlock2` directory, the script will automatically clone it from its GitHub repository.

## Usage

To start using the Sherlock scanner, navigate to the script directory and execute the script:

```bash
./sherlock2.sh
```

You will be presented with a menu of options:

1. **Basic Search**: Enter a single username to search across popular platforms.
2. **Multi-User Search**: Enter multiple usernames separated by spaces to search.
3. **Verbose Mode Search**: Perform a search that includes detailed logging.
4. **Search on All Platforms**: Conduct a comprehensive search across all supported platforms.

### Adding or Removing Platforms

Sherlock's GitHub repository regularly updates the list of supported platforms. To customize your searches, refer to the `sherlock2.py` script and the accompanying site data files in the Sherlock repository.

## FAQ

**Q: Do I need any special software to run the Sherlock scanner?**  
A: Yes, you need `git`, `Python 3`, and `pip`. The script will guide you through installing Sherlock itself.

**Q: Can I use this tool to search for usernames on any website?**  
A: Sherlock supports a wide range of websites, but its coverage is limited to those listed in its repository. You can contribute to the project by adding new sites.

**Q: How can I contribute to this project?**  
A: Contributions are welcome! Feel free to fork the repository, make your improvements, and submit a pull request.

---

For more information, updates, or to report issues, please visit the [Sherlock Project GitHub page](https://github.com/sherlock-project/sherlock).


Adjust the repository URL (`https://github.com/yourusername/SherlockScanner.git`) and any specific instructions as needed to align with your project's details. This document is designed to provide a clear and comprehensive guide for users to install, set up, and utilize the Sherlock scanner tool effectively.

## Contributing

We welcome contributions! Please follow these steps to contribute to darooch:

1. Fork the Project.
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`).
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the Branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

## Feedback and Support

For support, feedback, or suggestions, please open an issue in the GitHub repository. Your input helps make BashBuddy better for everyone.

### Final Steps

- Ensure you replace `https://github.com/shadowdevnotreal/OSINTtoolz.git` with the actual URL of your GitHub repository.
- Adjust any specific instructions or descriptions as needed based on your project's setup or requirements.
- If you have not already, consider adding a `LICENSE` file to clearly communicate how others can use or contribute to your project.

This README provides a comprehensive guide for users to get started, understand its features, and know how to contribute.

---

As always = TY 😊 

<a href="https://www.buymeacoffee.com/notarealdev">
    <img src="https://img.buymeacoffee.com/button-api/?text=Buy me a cat&emoji=🐈&slug=notarealdev&button_colour=9123cd&font_colour=ffffff&font_family=Bree&outline_colour=ffffff&coffee_colour=FFDD00" />
</a>
