# Getting Started with **Book Library**

This application demonstrates common use cases of **React Router**, including:

- Setting **dynamic parameters** in a URL and handling them accordingly.
- Using a **Private Route** to render components based on user authentication.
- Handling **404 Not Found** errors for unknown URLs.

The application fetches book data from `/public/books.json`, a static file containing **ID, title, author, and description** for each book.

---

## 📌 Available Routes

### **1. Home (`/`)**

- The `<Books>` component renders, displaying each book's **title and author** fetched from `books.json`.
- If the URL contains a **search query** (e.g., `/search?query=apple`), the app filters books by title **case-insensitively**.
  - Example: `/search?query=apple` will display all book titles containing "apple".
- **Note:** The search feature only works when accessing `/`.

### **2. Books (`/books`)**

- Redirects the user to `/`.

### **3. Book Details (`/books/:id`)**

- Displays details of a specific book, including **title, author, and description**, based on the given `id`.

### **4. Private Route (`/secret`)**

- If `isAuthenticated` is **true**, the `<SecretBooks>` component renders, displaying books accessible only to authorized users.
- If `isAuthenticated` is **false**, the user is redirected to `/`.
- **Note:** Authentication is a mock example and does not use a backend.

### **5. 404 Not Found (`*`)**

- Any other undefined route will render the `<NotFound>` component.

---

## 🔧 Available Scripts

Run the following commands in the project directory:

### **Install dependencies**

```sh
npm install
```

### **Start the development server**

```sh
npm start
```

Runs the app in development mode.  
Open [http://localhost:3000](http://localhost:3000) in your browser to view it.

---
