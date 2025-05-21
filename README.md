# 📅 Event Booking App - API Overview (FullStack App)

##  Introduction

This **Event booking management system** is a web-based platform that allows users to **create**, **manage**, and **register** for events.  

---

## Key Features

- **User Authentication** – Secure signup and login system.
- **Event Management** – Users can create, update, and delete events.
- **Event Registration** – Users can register and cancel their registration for events.
- **Access Control** – Only authenticated users can create, edit, or register for events.
- **CORS Handling** – Supports secure API access for both web and mobile applications.

---

##  Tech Stack

- **Go (Golang)** – Backend language
- **Chi Router** – Lightweight router for HTTP APIs
- **CORS Middleware** – Handles cross-origin resource sharing
- **Custom Repository Layer** – Abstracts storage operations (`repo.Storage`)

---

## Server Configuration

```go
srv := &http.Server{
	Addr:         ":8080",
	Handler:      mux,
	WriteTimeout: time.Second * 30,
	ReadTimeout:  time.Second * 10,
	IdleTimeout:  time.Minute,
}


# Clone the repo
git clone https://github.com/your-username/event-booking.git
cd event-booking

# Run the backend application
go run ./cmd

# Run the frontend application
cd web
npm install    (Go node modules)
npm run dev    (Start the development server)
