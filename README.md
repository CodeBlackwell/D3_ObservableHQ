# D3 ObservableHQ Notebook Downloader

A Node.js script to automatically download and extract D3.js examples and visualizations from ObservableHQ. This tool helps you easily obtain local copies of popular D3.js notebooks for learning, reference, or offline use.

## Features

- Automated downloading of ObservableHQ notebooks
- Progress bar visualization for download status
- Automatic extraction of downloaded notebooks
- Built-in delay between requests to respect server limits
- Support for multiple notebook downloads in a single run
- Colorful console output for better visibility
- Error handling and retry mechanisms

## Prerequisites

- Node.js (v14 or higher)
- npm (Node Package Manager)

## Installation

You can install this package either through npm or by cloning the repository.

### NPM Installation
```bash
npm install -g d3-observable-downloader
```

### Manual Installation
1. Clone this repository:
```bash
git clone https://github.com/codeblackwell/d3-observable-downloader.git
cd d3-observable-downloader
```

2. Install dependencies:
```bash
npm install
```

## Dependencies

- puppeteer - For web scraping and automation
- cli-progress - For progress bar visualization
- chalk - For colored console output
- tar - For handling .tgz files

## Usage

You can run the script in two ways:

1. If installed globally via npm:
```bash
d3-observable-download
```

2. If installed manually:
```bash
npm start
```

The script will:
1. Create a `resources` directory if it doesn't exist
2. Download specified ObservableHQ notebooks
3. Extract the downloaded notebooks
4. Show progress for each operation

## Included Notebooks

The script includes a curated list of popular D3.js notebooks, including:
- Animated Treemap
- Temporal Force-Directed Graph
- Connected Scatterplot
- The Wealth & Health of Nations
- Bar Chart Race
- Various visualization examples (treemaps, sunbursts, force-directed graphs, etc.)

## Project Structure

```
D3_ObservableHQ/
├── observables_scraper    # Main script
├── resources/            # Downloaded notebooks
└── README.md            # This file
```

## Configuration

The script includes a configuration object with the following defaults:
- Request delay: 1000ms
- Base URL: https://observablehq.com
- Downloads directory: User's system downloads folder

## Contributing

Feel free to submit issues, fork the repository, and create pull requests for any improvements.

## License

This project is open source and available under the MIT License.

## Acknowledgments

- ObservableHQ for providing the amazing D3.js examples
- D3.js community for creating these visualizations
