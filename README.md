# Automated-Daily-Expired-Password-Scraper

<h2>Step 1 - Create Script Folder</h2>

In Taskbar:

- Input File Explorer and open

Go to:

- This PC → Windows C: → New → Folder → Name Folder: Scripts

<p><img width="700" height="450" alt="image" src="https://github.com/user-attachments/assets/3f04f0dc-fe56-443c-82d4-15a631989706" />
</p>

<h2>Step 2 - Create Script File</h2>

Open Notepad:

In Taskbar:

- Input Notepad and open

In Notepad:

- Copy and paste this SCRIPT in it.

Save this script as DailyPasswordCheck.ps1

- File → Save as → This PC → Windows C: → Scripts

<p><img width="700" height="450" alt="image" src="https://github.com/user-attachments/assets/5e627167-6a90-4d0d-90a6-c0e212d17646" />
</p>

<h2>Step 3 - Task Scheduler Setup</h2>

In Taskbar:

- Input Task Scheduler and open

<p><img width="700" height="450" alt="image" src="https://github.com/user-attachments/assets/d9acf0e0-331d-4073-b45d-0d0b36820245" />
</p>

Go to Create Task:

<b>General tab</b>

- Name It:<b> Daily AD Password Expiration</b> 

Check: 

- Run whether user is logged on or not

- Run with highest privileges

<p><img width="700" height="450" alt="image" src="https://github.com/user-attachments/assets/5565f8fa-8db4-4cff-b7ba-cd850b7644c4" />
</p>

<b>Triggers tab</b>

Click <b>New</b>

- Begin the task: On a schedule

- Daily

- Start time: 7:00 AM 

<p><img width="700" height="450" alt="image" src="https://github.com/user-attachments/assets/50cf7652-c93c-43c6-a036-2c97b74ab05b" />
</p>

<b>Actions tab</b>

Click <b>New</b>

- Set <b>Program/script</b> to: <b>powershell.exe</b>

- Set <b>Add arguments</b> to:<b> -ExecutionPolicy Bypass -File "C:\Scripts\DailyPasswordCheck.ps1"</b>

<p><img width="700" height="450" alt="image" src="https://github.com/user-attachments/assets/e922d06d-07b5-4a39-982f-02021bec9f04" />
</p>

Click OK

- Enter your domain admin password

<p><img width="700" height="450" alt="image" src="https://github.com/user-attachments/assets/0b80fe14-ee63-4e3d-ad18-a5e9dbf04919" />
</p>

<h2>Step 3 - Check PasswordChangeReport</h2>

Open File Explorer:

- This PC → Windows C:

Open PasswordChangeReport

<p><img width="700" height="450" alt="image" src="https://github.com/user-attachments/assets/b50b359e-23f2-45f0-8b03-e9aff73ead9a" />
</p>

Observe thh PasswordChangeReport
