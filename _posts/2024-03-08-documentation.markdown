---
layout: post
title:  "IU Alumni Project Technical Documentation"
---

## Table of Contents

- [Overview](#Overview)
- [Regular Users](#Regular-Users)
    - [Pass Requests](#Pass-Requests)
    - [Elective Courses](#Electivec-courses)
    - [Make a Donation](#Donation)
    - [Account](#Account)
- [Developers](#Developers)
    - [Setup Instructions](#Setup-Instructions)
    - [Contributing](#Contributing)
    - [Deployment](#Deployment)
    
### Overview <a name="Overview"></a>
Welcome to the technical documentation for the IU Alumni project. The IU Alumni project is designed to help university students keep track of events, register for elective courses, manage attendance, and request passes for various university-related purposes. This documentation is split into two main sections: one for regular users and one for developers. 

### Technologies
- Frontend: Next.js, React
- Backend: Python FastAPI, PostgreSQL
- Deployment: Docker


## Getting Started

Before you can start using the IU Alumni project, you will need to log in or register.

### Logging In

If you already have an account, you can log in. Enter your email address and password, or use Innopolis SSO, and then click on the **Continue** button.

<p align="center">
  <img src="/myblog/images/Screenshot_9.png" />
</p>

### Registering

If you do not have an account, you can register by clicking on the **Register** link. Enter your email address, create a password, and then click on the **Continue** button.

Once you have logged in or registered, you will be able to access all of the features of the IU Alumni project.

## Regular Users <a name="Regular-Users"></a>


#### **Pass Requests** <a name="Pass-Requests"></a>

1. If you need to request a pass for university access, navigate to the **Pass Requests** section.
2. Fill out the required information and submit your request.

<p align="center">
  <img src="/myblog/images/Screenshot_8.png" />
</p>

Also you can see your requests history:
<p align="center">
  <img src="/myblog/images/Screenshot_13.png" />
</p>

And if click on button **View** you can see all details:
<p align="center">
  <img src="/myblog/images/Screenshot_14.png" />
</p>

#### **Elective Courses** <a name="Electivec-courses"></a>

1. To register for elective courses, go to the **Elective Courses** section of the website.
2. Select the course you want to register for and complete the registration process.
3. You can click **View** to see information about elective course.

<p align="center">
  <img src="/myblog/images/Screenshot_10.png" />
</p>

#### **Make a Donation** <a name="Donation"></a>

1. To make a donation, navigate to the **Make Donations** section of the IU Alumni website.
2. Click on the button **Send Donation Interest** or you can scan QR Code to make donation.

<p align="center">
  <img src="/myblog/images/Screenshot_11.png" />
</p>

#### **Account** <a name="Account"></a>

1. To change your data accounts, go to the **Account** section.
2. You will be able to see all fields and can change.

<p align="center">
  <img src="/myblog/images/Screenshot_12.png" />
</p>


## Developers <a name="Developers"></a>

### Setup Instructions <a name="Setup-Instructions"></a>

## Installing Frontend:

1. **Clone the Repository:** Use Git to clone the IU Alumni repository to your local machine.
2. Open a shell/command line in this folder
3. To `install` all packages (local to the repo) using `npm`
    ```bash
    npm install
    ```
4. To `build` the project for production
    ```bash
    npm run build
    ```
5. To `start` the project on development
    ```bash
    npm start
    ```

## Installing Backend

### Using Python
1. Open a shell/command line in this folder (better if it was after activating a python virtual env)
2. Install the needed python packages
```bash
    pip install -r requirements.txt
```
3. Run the python script:
```bash
    python3 main.py
```

### Using docker
1. Here the image tag name is `alumni-backend` you can name it as you like
2. Also the port in docker is 8000 by default and locally you can map it to anything as you like

```bash
docker build -t alumni-backend
docker run -p 8000:8000 -d alumni-backend
```

### Contributing <a name="Contributing"></a>

If you would like to contribute to the IU Alumni project, please follow these guidelines:

1. **Fork the Repository:** Fork the project repository to your GitHub account.
2. **Make Changes:** Create a new branch for your changes and make the necessary modifications.
3. **Submit a Pull Request:** Once you are done with your changes, submit a pull request to the main repository.

### Deployment <a name="Deployment"></a>

To deploy the IU Alumni project on a platform like Vercel, follow these steps:

1. **Create an Account:** Sign up for an account on Vercel and create a new project.
2. **Connect to Git:** Connect Vercel to your Git repository where the IU Alumni project is hosted.
3. **Configure Settings:** Configure the deployment settings as needed and deploy the project.

## Additional Resources

- [IU Alumni GitHub Repository](https://github.com/TheSharpOwl/inno-alumni-portal)
- [Vercel Documentation](https://vercel.com/docs)

Thank you for using the IU Alumni project! If you have any questions or need further assistance, please don't hesitate to reach out to us.
