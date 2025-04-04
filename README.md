## 🌐 API Endpoints

### 1️⃣ Get All Names

**Method**: `GET`  
**URL**: `http://127.0.0.1:8000/`  
📦 **Returns** a list of all names.

**Example Response:**
```json
["Taha", "Raza", "Ali"]
```

---

### 2️⃣ Add a New Name

**Method**: `POST`  
**URL**: `http://127.0.0.1:8000/`  
📨 **Send JSON body like:**
```json
{
  "name": "Zain"
}
```

**✅ Response (updated list):**
```json
["Taha", "Raza", "Ali", "Zain"]
```

---

### 3️⃣ Delete a Name

**Method**: `DELETE`  
**URL**: `http://127.0.0.1:8000/{name}`  
🗑️ Replace `{name}` with the name you want to delete.

**Example**:  
`DELETE http://127.0.0.1:8000/Raza`

**✅ Response (updated list):**
```json
["Taha", "Ali"]
```

---

### 4️⃣ Update a Name

**Method**: `PUT`  
**URL**: `http://127.0.0.1:8000/{name}`  
✏️ Replace `{name}` with the name you want to change.  
📨 Send JSON body like:
```json
{
  "name": "Bilal"
}
```

**Example**:  
`PUT http://127.0.0.1:8000/Ali`

**✅ Response (updated list):**
```json
["Taha", "Raza", "Bilal"]
```

---

## 🧠 Notes

- All names are stored in memory (a list), so they reset when you stop the server.
- This API is simple and good for learning! 🧑‍💻

---

Enjoy using the API! ✨  
Made with ❤️ and FastAPI 🚀
