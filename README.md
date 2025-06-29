# Historical Polish Audiobook Finder

![Node.js](https://img.shields.io/badge/Node.js-18.x-green)
![License](https://img.shields.io/badge/License-MIT-blue)
![Status](https://img.shields.io/badge/Status-Maintained-brightgreen)

A Node.js web scraping tool that searches for audiobook versions of historical Polish books listed in the Polona digital library.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Technical Stack](#technical-stack) 
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Error Handling](#error-handling)
- [Legal Notice](#legal-notice)
- [License](#license)

## Overview

This project automates the process of:
- Fetching historical Polish book metadata from the Polona.pl API
- Searching Google for potential audiobook versions on Polish government websites
- Analyzing search results to identify exact matches
- Downloading and parsing PDFs, Excel files, and Word documents when found
- Handling rate limiting and network errors gracefully

## Features

### Advanced Scraping
- Uses Puppeteer with stealth plugin to avoid detection
- Rotates user agents to prevent blocking
- Implements random delays between requests

### Robust Processing
- Parses multiple file formats:
  - PDF (using pdf-parse)
  - Excel (using xlsx)
  - Word (using mammoth)
  - CSV (using csv-parse)

### Comprehensive Monitoring
- Automatic 429 error detection
- Audio notifications for rate limits
- Connection monitoring and auto-recovery
- Detailed JSON logging system

## Technical Stack

| Component | Technology |
|-----------|------------|
| Runtime | Node.js |
| Scraping | Puppeteer + Cheerio |
| HTTP Client | Axios |
| PDF Parsing | pdf-parse |
| Excel Parsing | xlsx | 
| Word Parsing | mammoth |
| CSV Parsing | csv-parse |
| Audio Alerts | audio-play |

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/audiobook-finder.git
cd audiobook-finder
