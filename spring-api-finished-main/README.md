# 🛍️ Ecommerce Backend – Spring Boot API

This repository contains the **backend code** for my Spring Boot-based e-commerce application. It’s designed with a focus on clean RESTful API architecture, secure authentication, Stripe integration, and database migrations. The project is a hands-on demonstration of mastering modern Spring Boot API development.

> 👨‍💻 Author: [Harsh Jaiswal](https://github.com/HarshJaiswal497)

---

## ⚙️ Tech Stack

- Java 17
- Spring Boot
- Spring Security + JWT
- Spring Data JPA + Hibernate
- Flyway (Database Migrations)
- Stripe (Payment Gateway)
- MySQL / H2
- Swagger (API Docs)

---

## 🚀 Features

- 🔐 User Registration & JWT Login
- 📦 Product Management
- 🛒 Cart Management (Create, Add Items)
- 💳 Checkout with Stripe
- 🧾 Order Tracking
- 🔁 Stripe Webhooks for Real-Time Order Updates
- 📘 Auto-Generated API Docs with Swagger

---

## 🛠️ Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/HarshJaiswal497/Ecommerce_Backend_SpringBoot.git
cd Ecommerce_Backend_SpringBoot
```

---

### 2. Setup Environment Variables

Create a `.env` file using `.env.example` as a template. It should include the following keys:

#### 🔑 JWT_SECRET
Generate a secure token using:

```bash
openssl rand -base64 32
```

Or use a tool like [generate-random.org](https://generate-random.org) for API tokens.

#### 💳 STRIPE_SECRET_KEY
- Sign up at [Stripe](https://stripe.com)
- Go to **Developers → API Keys**
- Copy your **Secret Key**

#### 📬 STRIPE_WEBHOOK_SECRET_KEY
Install Stripe CLI and run the following:

```bash
stripe login
stripe listen --forward-to http://localhost:8080/checkout/webhook
```

Copy the **signing secret** from the terminal and set it in your `.env`.

---

### 3. Running the Application

This is a Maven project. To run the application:

#### On Linux/Mac:

```bash
./mvnw spring-boot:run
```

#### On Windows:

```bash
mvnw.cmd spring-boot:run
```

The server will start at:
```
http://localhost:8080
```

---

### 📚 API Documentation

Swagger UI is available at:
```
http://localhost:8080/swagger-ui.html
```

---

## 📦 Folder Structure (Optional)


---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🙌 Connect With Me

- [LinkedIn](https://www.linkedin.com/in/harshjaiswal01/)
- [Portfolio](https://portfolioharshjaiswal.netlify.app/)