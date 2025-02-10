---

# Facebook Incoming Item Scraper  

## **Login Process**  
1. Check if Facebook is already logged in.  
   - If logged in, continue without re-authentication.  
   - If not logged in, retrieve credentials from `credentials.csv` and log in.  
   - Save cookies for future logins.  
2. Handle Facebook's security measures:  
   - If approval or a verification code is required, wait for input instead of stopping with an error.  
   - Ensure smooth error handling.  

## **Input File Processing**  
1. **Direct URL Usage**:  
   - If `input_url.txt` contains a URL, use it directly without applying marketplace filters.  
2. **Filtered Search**:  
   - If no URL is available, apply filters from `input_file.csv` to the Facebook Marketplace.  
   - Search the same filters across all locations listed in `location.txt` and extract relevant data.  
3. **Time-Based Extraction**:  
   - Extract only items uploaded within the last 24 hours.  

## **Output Format**  
- The extracted data should match the structure of the provided sample file.  

## **Additional Features**  
- **Automatic Account Switching**:  
  - Change login (using cookies) after extracting 20–30 products to avoid Facebook blocking the account.  
- **Undetectable & User-Friendly**:  
  - Ensure the scraper runs smoothly without detection.  
  - Implement robust error handling and retries.  
- **Server Deployment**:  
  - The scraper must be able to run continuously for **5–6 hours daily** on a server.  
- **Thorough Testing**:  
  - Test multiple times to eliminate errors and ensure stability.  

## **Reference Screenshot**  
- ![Screenshot](https://github.com/user-attachments/assets/d10eb4d8-1091-4237-87d2-4144e0e8bc93)  

---
