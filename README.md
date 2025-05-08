# WT Project

This is a full-stack monorepo containing:

- `frontend/` – React (Vite) application
- `backend/` – Spring Boot application

## 🛠️ Prerequisites

Make sure you have the following installed:

- [Node.js](https://nodejs.org/) (v16 or later recommended)
- [Java JDK](https://adoptopenjdk.net/) (v17 or later)
- [Maven](https://maven.apache.org/) (or use mvnw from spring boot project initializer)

---

## 🚀 Cloning the Repository

This repo uses Git **submodules** for `frontend` and `backend`.

```bash
git clone --recurse-submodules https://github.com/yourname/wt.git
cd wt/
```

If you forget `--recurse-submodules`, run:

```bash
git submodule update --init --recursive
```

---

## 📦 Installing Dependencies

### Frontend (React + Vite)

```bash
cd frontend
npm install
```

### Backend (Spring Boot + Maven)

```bash
cd ../backend
mvn clean install
```

---

## ▶️ Running the Apps

### Frontend (React Dev Server)

```bash
cd frontend
npm run dev
```

This will start the frontend on [http://localhost:5173](http://localhost:5173)

### Backend (Spring Boot Server)

```bash
cd backend
mvn spring-boot:run
```

By default, the backend runs on [http://localhost:8080](http://localhost:8080)

---

## 📁 Project Structure

```
wt/
├── frontend/      # React (Vite) project
├── backend/       # Spring Boot project
└── .gitmodules    # Tracks submodules
```

---

## 🧪 Tips

- Make sure the frontend is configured to make API requests to `http://localhost:8080` (or use a proxy if needed).
- Use `.env` files for environment-specific configs.

---

## 📝 License


