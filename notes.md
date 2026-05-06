# Notes

## Project Setup

### Backend Setup

[ ] Create `server` folder  
[ ] Initialize Node.js project

```bash
npm init -y
```

[ ] Install backend dependencies

```bash
npm install express mongoose dotenv cors body-parser
```

[ ] Install nodemon

```bash
npm install --save-dev nodemon
```

[ ] Create folders:

- `controller`
- `model`
- `routes`

[ ] Create files:

- `index.js`
- `.env`
- `userController.js`
- `userModel.js`
- `userRoute.js`

---

## Frontend Setup

[ ] Create React application

```bash
npx create-react-app client
```

[ ] Install frontend dependencies

```bash
npm install axios react-router-dom bootstrap font-awesome
```

[ ] Create component folders:

- `addUser`
- `getUser`
- `updateUser`
- `deleteUser`

[ ] Create component files:

- `AddUser.jsx`
- `User.jsx`
- `Update.jsx`
- `Delete.jsx`

[ ] Create CSS files:

- `addUser.css`
- `user.css`
- `update.css`
- `delete.css`

---

# MongoDB Notes

[ ] Install MongoDB locally  
[ ] Open MongoDB Compass  
[ ] Create local database:

- `mern-app`

[ ] Create `.env` file inside `server`

```env
PORT=8000
MONGO_URL=mongodb://localhost:27017/mern-app
```

---

# Express Notes

## Main Server Setup

```js
app.use(express.json());
app.use(cors());
```

MongoDB connection:

```js
mongoose.connect(MONGO_URL);
```

Start server:

```bash
node index.js
```

or:

```bash
npm start
```

---

# React Router Notes

Install router:

```bash
npm install react-router-dom
```

Routes used:

```js
"/";
"/add";
"/update/:id";
"/delete/:id";
```

Router setup inside:

```bash
App.js
```

---

# Axios Notes

Install axios:

```bash
npm install axios
```

Used for:

- GET requests
- POST requests
- PUT requests
- DELETE requests

Example:

```js
axios.get();
axios.post();
axios.put();
axios.delete();
```

---

# CRUD Notes

## Create User

Method:

```http
POST /api/user
```

---

## Get Users

Method:

```http
GET /api/users
```

---

## Update User

Method:

```http
PUT /api/user/:id
```

---

## Delete User

Method:

```http
DELETE /api/user/:id
```

---

# CSS Notes

Main concepts used:

- Flexbox
- Responsive layout
- Media queries
- Hover effects
- Shadows
- Button transitions

---

# Important Commands

## Start Backend

```bash
cd server
npm start
```

If npm start does not work:

```bash
node index.js
```

---

## Start Frontend

```bash
cd client
npm start
```

---

# Common Errors

## MongoDB Connection Error

Possible reasons:

- MongoDB server not running
- Wrong MONGO_URL
- Missing `.env` file

---

## CORS Error

Possible reason:

- Backend missing cors middleware

Solution:

```js
app.use(cors());
```

---

## Port Already In Use

Possible reason:

- Another application using same port

Change port inside `.env`

---

# Personal Learning Notes

Things practiced in this project:

- MERN stack structure
- REST API development
- MongoDB CRUD operations
- React routing
- Axios API requests
- Express controllers
- Responsive CSS
- Full-stack application workflow
