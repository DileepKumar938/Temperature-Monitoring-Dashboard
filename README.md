# Temperature-Monitoring-Dashboard

🚀 A React + .NET Core web application to monitor and control temperature variations using real-time sensor data.  

---

## 📌 Features  
✅ Real-time temperature monitoring  
✅ API integration for data collection  
✅ Dashboard UI using React.js
✅ Backend with .NET Core & Web API  
✅ SQL Server for data storage  

---

## 📂 Project Setup (Step-by-Step Guide)  

### 1️⃣ Clone the Repository
```sh
git clone https://github.com/your-username/Temperature-Monitoring-Dashboard.git
cd Temperature-Monitoring-Dashboard
```

---

## 🖥️ Backend Setup (.NET Core API)

### 2️⃣ Install .NET Core SDK
[Download .NET SDK](https://dotnet.microsoft.com/download)  

### 3️⃣ Create and Set Up API 
```sh
cd backend
dotnet new webapi -n SmartTempAPI
cd SmartTempAPI
```

### 4️⃣ Install Dependencies
```sh
dotnet add package Microsoft.EntityFrameworkCore.SqlServer
dotnet add package Microsoft.AspNetCore.Cors
```

### 5️⃣ Configure Database (SQL Server) 
- Modify `appsettings.json` with your SQL Server connection string  
- Run the following command to apply migrations:  
```sh
dotnet ef migrations add InitialCreate
dotnet ef database update
```

### 6️⃣ Run the API Server  
```sh
dotnet run
```
Your API will run on `http://localhost:5000/api/temperature`  

---

## 🌐 Frontend Setup (React.js)  

### 7️⃣ Install Node.js & React
[Download Node.js](https://nodejs.org/)  

```sh
cd frontend
npx create-react-app temp-monitor-dashboard
cd temp-monitor-dashboard
```

### 8️⃣ Install Required Libraries  
```sh
npm install axios chart.js bootstrap
```

### 9️⃣ Configure API in React
- Update `src/config.js` with API URL  
```js
export const API_URL = "http://localhost:5000/api/temperature";
```

### 🔟 Start the React App
```sh
npm start
```
Open `http://localhost:3000` in your browser.  

---

## 📌 Repository Structure 
```
Temperature-Monitoring-Dashboard/
│── backend/          # .NET Core Web API
│── frontend/         # React.js App
│── README.md         # Project Documentation
│── LICENSE           # Open-source License
```

---

## 📢 How to Contribute? 
1. Fork the repository  
2. Create a feature branch (`git checkout -b feature-name`)  
3. Commit changes (`git commit -m "Added new feature"`)  
4. Push to GitHub (`git push origin feature-name`)  
5. Create a Pull Request  

---

