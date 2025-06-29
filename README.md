# 🏅 Contest Registration System

A simple web-based system to allow users to register for contests, list available contests, and manage registrations.

---

## 🔍 Table of Contents
- [About the Project](#about-the-project)  
- [Features](#features)  
- [Tech Stack](#tech-stack)  
- [Setup & Installation](#setup--installation)  
- [Usage](#usage)  
- [Project Structure](#project-structure)  
- [Contributing](#contributing)  
- [License](#license)  
- [Contact](#contact)

---

## 📖 About the Project

This project simplifies the process of contest registration:
- Users can **view all contests**, **sign up**, and **cancel registrations**.
- Admins can add, edit, or delete contests.
- Ideal for coding competitions, hackathons, or school events.

---

## ⚙️ Features

- List all available contests  
- Register/unregister for contests  
- Admin functionality to **add**, **edit**, and **remove** contests  
- Input validation and error handling  
- Designed for easy frontend integration or API extension

---

## 🛠️ Tech Stack

- **Backend**: [Node.js](https://nodejs.org/) + [Express](https://expressjs.com/)  
- **Database**: JSON-based storage (no external DB dependency)  
- **Language**: JavaScript (ES6+)

---

## 🧰 Setup & Installation

1. **Clone the repo**
   ```bash
   git clone https://github.com/akilan200/Contest_Registration.git
   cd Contest_Registration
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Run the app**
   ```bash
   npm start
   ```
   The server should start on `http://localhost:3000`.

---

## 🎯 Usage

Use an API client (e.g., Postman) or browser to make calls:

| Endpoint                    | Method | Description                     |
|-----------------------------|--------|---------------------------------|
| `/contests`                | GET    | Get all contests                |
| `/contests/:id`            | GET    | Get contest by ID               |
| `/contests`                | POST   | Add a new contest               |
| `/contests/:id/register`   | POST   | Register user for contest       |
| `/contests/:id/unregister` | POST   | Cancel registration             |

Example request to create a new contest:
```json
{
  "name": "Hackathon 2025",
  "date": "2025-07-15",
  "description": "A 24-hour coding event."
}
```

---

## 🗂️ Project Structure

```
.
├── controllers/         # API logic
├── data/                # JSON files (contests + registrations)
├── routes/              # Express route definitions
├── models/              # Data models
├── app.js               # Main Express app
└── package.json         # Dependencies & scripts
```

---

## 🤝 Contributing

Contributions are welcome!

1. Fork this project  
2. Create a branch (`git checkout -b feature/YourFeature`)  
3. Make changes & commit (`git commit -m 'Add some feature'`)  
4. Push (`git push origin feature/YourFeature`)  
5. Open a Pull Request

Please follow clean code styles and include tests wherever possible.

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 📬 Contact

- **Project Author**: [akilan200](https://github.com/akilan200)  
- **Email**: akilanlh2004@gmail.com

---
