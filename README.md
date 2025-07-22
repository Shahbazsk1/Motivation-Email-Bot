# Motivation-Email-Bot
<h2>To send a random motivational quote from a text file (quotes.txt) to your email every Monday, helping you or others start the week on a positive note.
</h2>
<h3>📁 Project Files Structure:</h3>
<p>
  monday_motivation/<br>
│
├── main.py                 # Main Python script<br>
├── quotes.txt              # Text file with motivational quotes (1 per line)<br>
</p>
<h3>Modules Used:</h3>
<ul>
  <li><b>smtplib :</b>	Used to connect and send emails via SMTP (Simple Mail Transfer Protocol).</li>
  <li><b>datetime :</b>	Gets the current date and checks what day of the week it is.</li>
  <li><b>random :</b>	Picks a random motivational quote from the list.</li>
</ul>
<h4>🔐 Security Note:</h4>
<p>
  MY_EMAIL = "youremail@gmail.com"<br>
  MY_PASSWORD = "your_app_password"<br>
</p>
<ul>
  <li>Never share your real Gmail password in code.</li>
  <li>Use Gmail App Passwords for this.</li>
  <li>Alternatively, store credentials securely in environment variables or a .env file.</li>
</ul>
