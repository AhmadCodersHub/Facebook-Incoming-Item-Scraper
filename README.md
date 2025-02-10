Facebook-Incoming-Item-Scraper:
  Login the Facebook:
    - "First, check if Facebook is logged in or not."
    - "If Facebook is already logged in, no need to log in again."
    - "If not logged in, retrieve credentials from 'credentials.csv' and log in."
    - "Save cookies for future logins."
    - "Handle errors properly: If Facebook asks for verification (like a security code), the script should wait instead of stopping with an error."

  Inputs File Information:
    - "If 'input_url.txt' contains a URL, use it directly (no need to apply marketplace filters)."
    - "If 'input_url.txt' is empty, apply filters from 'input_file.csv' to search the Facebook Marketplace."
    - "If input URL is missing, search using filters across all locations listed in 'location.txt'."
    - "Extract all items uploaded in the last 24 hours."

  Output:
    - "The extracted data should match the format of the provided sample file."

  Additional Features:
    - "Automatically switch accounts using cookies after extracting 20–30 products to avoid Facebook blocking."
    - "Ensure the bot is user-friendly and undetectable."
    - "Test multiple times to eliminate all possible errors."
    - "Deploy the bot on a server and run it for 5–6 hours daily."

  Reference Screenshot:
    - ![Screenshot](https://github.com/user-attachments/assets/d10eb4d8-1091-4237-87d2-4144e0e8bc93)
