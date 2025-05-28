# OWASP Juice Shop - Local Deployment Guide (Linux, Node.js)

This guide provides step-by-step instructions to deploy the [OWASP Juice Shop](https://github.com/juice-shop/juice-shop) web application locally on a Linux system using Node.js.

---

## 📋 Prerequisites

Before you begin, ensure the following dependencies are installed on your Linux machine:

* **Node.js** (version 16.x or above recommended)
* **npm** (comes with Node.js)
* **git**

### Install Node.js and npm (if not already installed)

```bash
sudo apt update
sudo apt install nodejs npm -y
```

Verify installation:

```bash
node -v
npm -v
```

---

## 📁 Clone the Repository

Clone the official Juice Shop repository or fork and clone your own copy:

```bash
git clone https://github.com/juice-shop/juice-shop.git
cd juice-shop
```

---

## 📦 Install Dependencies

Install the required Node.js packages:

```bash
npm install
```

This will download all dependencies listed in the `package.json` file.

---

## 🚀 Start the Application

To run the Juice Shop app locally:

```bash
npm start
```

The application will build and start a local server, typically accessible at:

```
http://localhost:3000
```

You should see a welcome page for OWASP Juice Shop.

---

## 🛠️ Custom Configuration (Optional)

You can customize the configuration using a `.env` file or environment variables. Example:

```bash
echo "PORT=4000" > .env
```

Then restart the app with:

```bash
npm start
```

Now it will be accessible at `http://localhost:4000`.

---

## 🧲 Testing the Setup

Once the app is running:

1. Open a browser and go to `http://localhost:3000` (or your configured port).
2. You should see the Juice Shop welcome screen.
3. Interact with the application to test various vulnerabilities.

---

## 𞲠 Stopping the App

To stop the app, press:

```
Ctrl + C
```

in the terminal window running the app.

---

## 📚 Useful Resources

* [Official OWASP Juice Shop GitHub Repo](https://github.com/juice-shop/juice-shop)
* [Documentation and Hacking Guide](https://pwning.owasp-juice.shop/)
* [OWASP Juice Shop CTF Extension](https://github.com/juice-shop/juice-shop-ctf)

---

## 📄 License

This project is licensed under the [MIT License](https://github.com/juice-shop/juice-shop/blob/master/LICENSE).

---
