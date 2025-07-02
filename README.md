## Historical Polish Audiobook Finder  
**Status: Development**  
![Tech](https://img.shields.io/badge/-Node.js-339933) ![Tech](https://img.shields.io/badge/-Puppeteer-40B5A4) ![Tech](https://img.shields.io/badge/-Axios-5A29E4)  

🖼️ **Preview**:  
![App Preview](https://cdn.glitch.global/5ac0b5d5-9cdf-4f57-b49d-3e7a215b66a4/logs.png)  

### ✨ Features  

#### Advanced Scraping  
- Uses Puppeteer with stealth plugin  
- Rotates user agents  
- Implements random delays  

#### Robust Processing  
- Parses multiple formats:  
  - PDF (pdf-parse)  
  - Excel (xlsx)  
  - Word (mammoth)  
  - CSV (csv-parse)  

#### Comprehensive Monitoring  
- 429 error detection  
- Audio notifications  
- Connection auto-recovery  
- JSON logging  

### 🛠️ Technical Stack  
| Component         | Technology                          |
|-------------------|-------------------------------------|
| Runtime          | Node.js ![Node.js](https://img.shields.io/badge/-Node.js-339933) |
| Scraping        | Puppeteer + Cheerio ![Puppeteer](https://img.shields.io/badge/-Puppeteer-40B5A4) |
| HTTP Client     | Axios ![Axios](https://img.shields.io/badge/-Axios-5A29E4) |
| PDF Parsing     | pdf-parse |
| Excel Parsing   | xlsx |
| Word Parsing    | mammoth |
| CSV Parsing     | csv-parse |
| Audio Alerts    | audio-play |

### 📝 Notes  
```mermaid
graph TD
    A[Polona.pl API] -->|Get Book Metadata| B(Search Gov Portals)
    B --> C{Found Audiobooks?}
    C -->|Yes| D[Verify Match]
    C -->|No| E[Log as Unavailable]
    D --> F[Store Results]
- Scrapes government sites for audiobook versions  
- Handles rate limiting gracefully  
