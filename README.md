# 📧 Jenkins Email Notification & Git Clone Job

This project demonstrates how to **configure Jenkins email notifications** and create a **Git repository cloning job** with post-build email alerts for both success and failure events.  
It helps developers stay updated about Jenkins build results directly in their mailbox. 📬

---

## 🚀 Project Overview

In this project, I performed the following tasks:

1. **Configured Jenkins Email Notification (SMTP setup)**
2. **Tested the email functionality**
3. **Created a Jenkins job (`clone-job`) to clone a GitHub repository**
4. **Added developer email in Post-Build Actions**
5. **Received two types of emails:**
   - ✅ **Success Email** when the job succeeded
   - ❌ **Failure Email** when the job failed

---

## 🛠️ Tools & Technologies Used

- **Jenkins** 🧩  
- **GitHub** 💻  
- **SMTP Mail Configuration** ✉️  
- **Ubuntu / Linux Environment** 🐧  

---

## ⚙️ Step-by-Step Implementation

### 1️⃣ Configure Jenkins Mail Server (SMTP)

- Go to **Manage Jenkins → Configure System**
- Scroll to **E-mail Notification** section
- Add your mail credentials (SMTP server, port, username, password)
- Enable **Use SMTP Authentication** and **Use SSL/TLS**
- Click **Test Configuration by sending a test e-mail**

📸 *Screenshot:* SMTP Configuration and Test Email
![](/images/Screenshot%20(755).png)
![](/images/Screenshot%20(756).png)
![](/images/Screenshot%20(757).png)
![](/images/Screenshot%20(758).png)

---

### 2️⃣ Create a New Job — `clone-job`

- Click on **New Item → Freestyle Project**
- Enter job name: `clone-job`
- Choose **Freestyle project** and click **OK**

📸 *Screenshot:* New Job Setup

---

### 3️⃣ Configure Git Repository

- Go to **Source Code Management → Git**
- Add your **GitHub Repository URL**
- If private, add credentials
- Save configuration

📸 *Screenshot:* Git Configuration
![](/images/Screenshot%20(752).png)
![](/images/Screenshot%20(753).png)

---

### 4️⃣ Add Post-Build Email Notification

- Scroll to **Post-build Actions**
- Choose **E-mail Notification**
- Add developer’s email ID (e.g., `developer@example.com`)
- Configure triggers:
  - Send email on **Failure**
  - Send email on **Success**

📸 *Screenshot:* Post-Build Email Configuration
![](/images/Screenshot%20(754).png)

---

### 5️⃣ Run the Job and Test Email Alerts

- Click **Build Now**
- Observe console output and email inbox for results:
  - ✅ Success Email → Job cloned and completed successfully  
  - ❌ Failure Email → Error occurred while cloning repository

📸 *Screenshot:* Email received for success and failure
![](/images/Screenshot%20(763).png)
![](/images/Screenshot%20(766).png)

---

## 📂 Project Structure
📁 Jenkins-Email-Notification

- ┃ ┣ smtp-setup
- ┃ ┣ clone-job
- ┃ ┣ post-build-action
- ┃ ┣ success-mail
- ┃ ┗ failure-mail


---

## 🎯 Outcome

- Jenkins successfully sent emails to the developer on both **job success** and **failure**.
- Demonstrated **automation of email notifications** using Jenkins Post-Build Actions.
- Verified smooth **integration of Jenkins with GitHub** and **email alerts**.

---

## 🧠 Learning Highlights

- How to configure SMTP in Jenkins  
- How to test and verify email notifications  
- How to create and manage Git-based Jenkins jobs  
- How to automate build notifications for developers  

---

## 🏁 Conclusion

This project shows the **complete lifecycle of email automation in Jenkins**, from configuration to testing.  
It’s a simple yet powerful demonstration of **Continuous Integration + Notification System** for developers.

---

## 👨‍💻 Author

**Vivek Chopade**  
*DevOps & Cloud Engineer | MCA Student*  
📧 [Email Me](chopadevivek4466@gmail.com)  
🌐 [GitHub Profile](https://github.com/chopadevivek07)


---
