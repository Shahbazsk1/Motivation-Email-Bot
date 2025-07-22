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

<h3>✅ Step-by-Step: Use Gmail App Password</h3>
<ol>
  <li>
    <strong>Enable 2-Step Verification on Your Google Account</strong><br>
    App passwords only work if 2FA is enabled.<br><br>
    Go to: 
    <a href="https://myaccount.google.com/security" target="_blank">
      https://myaccount.google.com/security
    </a><br><br>
    Under “Signing in to Google”, enable 2-Step Verification
  </li>
  <br>
  <li>
    <strong>Generate App Password</strong><br>
    After enabling 2FA, go to: 
    <a href="https://myaccount.google.com/apppasswords" target="_blank">
      https://myaccount.google.com/apppasswords
    </a><br><br>
    Select <code>Mail</code> as the app and <code>Windows Computer</code> (or other) as the device<br>
    Click <strong>Generate</strong><br><br>
    Google will give you a 16-character password like:<br>
    <code>abcd efgh ijkl mnop</code>
  </li>
  <br>
  <li>
    <strong>Use the App Password in Your Script</strong><br>
    Update your script like this:<br><br>
    <pre><code>MY_EMAIL = "yourgmail@gmail.com"
  MY_PASSWORD = "abcd efgh ijkl mnop"  # Your app password here</code></pre>
  </li>
</ol>
