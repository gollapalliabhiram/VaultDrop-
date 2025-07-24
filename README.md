
# 🔐 VaultDrop – Secure File Sharing Platform

**VaultDrop** is a backend-focused file-sharing platform that allows users to securely upload, share, and download files via unique expirable links. It supports SMTP-based email notifications and automated cleanup for enhanced performance and security.

---

## 🚀 Tech Stack

- **Backend**: Node.js, Express.js  
- **Database**: MongoDB  
- **File Uploads**: Multer  
- **Email Service**: Nodemailer (SMTP)  

---

## ✨ Features

- 📤 Upload and share files with unique download links  
- 📧 Email-based file sharing with customizable SMTP templates  
- ⏲️ Auto-delete files after 24 hours using scheduled jobs  
- 🔐 Download tracking and secured file access routes  

---

## 🛠️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/vaultdrop-.git
cd vaultdrop
````

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment Variables

Create a `.env` file and add:

```env
PORT=
MONGODB_URI=
BASE_URL=
SMTP_HOST=
SMTP_PORT=
SMTP_USER=
SMTP_PASS=
```

### 4. Run the App Locally

```bash
npm start
```

### 5. Schedule File Cleanup (Production)

Configure a daily job on **Heroku Scheduler** to delete expired files:

```bash
node services/deleteOldFiles.js
```

---

## 📦 Key Functionalities

### 📤 File Upload & Storage

* Uses Multer to handle file uploads
* Stores file metadata and expiration in MongoDB
* Generates unique IDs for secure file access

### 📧 Email Sharing

* Sends email with download link using Nodemailer + SMTP
* Supports HTML templates for professional emails

### 🗑️ Auto-Cleanup (Cron Jobs)

* Scheduled script deletes files older than 24 hours
* Keeps the server clean and efficient

---

## 👤 Author

**Gollapalli Abhiram**
🔗 [LinkedIn](https://www.linkedin.com/in/abhiramgollapalli/)
🔗 [GitHub](https://github.com/gollapalliabhiram)

