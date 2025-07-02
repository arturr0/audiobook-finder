## Historical Polish Audiobook Finder  
**Status: Development**  
![Tech](https://img.shields.io/badge/-Node.js-339933) ![Tech](https://img.shields.io/badge/-Puppeteer-40B5A4) ![Tech](https://img.shields.io/badge/-Axios-5A29E4)  

 ![App Preview](https://cdn.glitch.global/79283f6f-ef1e-4285-822b-eaefe68c462e/5.png?v=1751443834188)  

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
**Data Ingestion**:  
- Fetches metadata of public domain Polish works from Polona API  
- Scrapes government sites for audiobook versions  
- Handles rate limiting gracefully  
