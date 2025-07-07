<div align="center">

# Alexa Google Sheets 🎤  
*Seamlessly interact with your Google Sheets using natural voice commands through Alexa!*

</div>


---

## 🌟 Introduction  
Transform how you interact with spreadsheets! This innovative Alexa Skill bridges voice technology and Google Sheets, allowing you to **read**, **write**, and **search** data using natural voice commands. Perfect for hands-free data management during cooking, driving, or multitasking!


---

## ✨ Key Features  

| Feature | Description | Example Command |
|---------|-------------|-----------------|
| **📖 Read Cells** | Retrieve values from any cell | *"Read cell C10"* |
| **✍️ Write Data** | Update cells with voice input | *"Write 'Meeting at 3PM' in A2"* |
| **🔍 Search Sheets** | Find text across your spreadsheet | *"Search for 'Annual Budget'"* |
| **🗣️ Natural Interaction** | Conversational commands | *"What's in the top-left cell?"* |


---

## 🛠️ Setup Guide  

### Prerequisites  
1. ✅ **Amazon Developer Account**  
2. ✅ **Google Cloud Console** with Sheets API enabled  
3. ✅ Python 3.8+ environment  

### Installation  
```bash
# Clone repository
git clone https://github.com/<your-repo>/Alexa-sheets.git
cd Alexa-sheets


```

### Configuration  
1. **Google Sheets Setup**  
   - Create service account credentials  
   - Share your Google Sheet with the service account email  
   - Add `credentials.json` to `lambda/` directory  

2. **Alexa Skill Configuration**  
   ```python
   # In lambda/handlers/config.py
   SHEET_ID = "your-google-sheet-id"
   API_SCOPES = ['https://www.googleapis.com/auth/spreadsheets']
   ```

### Deployment  
1. Zip Lambda handlers:  
   ```bash
   cd lambda && zip -r ../alexa-sheets.zip *
   ```
2. Upload to AWS Lambda Console  
3. Build interaction model in Alexa Developer Console using `interactionModels/custom` files  

---

## 🚀 Future Capability Integration

- **Multi-Sheet Navigation**  
  *"Switch to Inventory Sheet"*  
- **Row/Column Operations**  
  *"Add new row below position 5"*  
- **Data Visualization**  
  *"Create pie chart from A1 to B10"*  
- **Error Resilience**  
  Improved handling for invalid cell references  

---

## 📜 License  
Distributed under the MIT License. See `LICENSE` for more information. 
---

**Contribute**: Feel free to submit issues!  

