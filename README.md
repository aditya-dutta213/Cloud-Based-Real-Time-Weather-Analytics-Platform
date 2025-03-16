# **Weather Forecast Web & Mobile Applications** 🌦️📱  
**Technologies:** Angular, Node.js, MongoDB, Google Cloud, Tomorrow.io API, Android Studio, Java, HighCharts  

🚀 **Live Web App:** [Weather Search](https://weather-search-project.wl.r.appspot.com/)  
🌍 **Backend API Endpoint:** [Sample Query](https://backend-dot-weather-search-project.wl.r.appspot.com/get_weather?city=Los+Angeles&state=CA)  
📱 **Android App Demo:** *(Video uploaded to repository)*  

---

## **Project Overview**  
This project includes a **web application (HW3)** and an **Android app (HW4)** for real-time **weather forecasting** using the **Tomorrow.io API**. Both platforms allow users to **search weather, view forecasts, save favorite locations, and share updates on Twitter/X**.  

### **Key Features**  
✅ **Web App (Angular + Node.js + MongoDB)**  
- Weather search via **city/state input** or **auto-detect location**  
- Displays **current conditions, 7-day forecast, and interactive charts**  
- **MongoDB Atlas** stores favorite cities  
- Twitter **Web Intents** for sharing weather updates  
- **Google Cloud Deployment (App Engine + MongoDB Atlas)**  

✅ **Android App (Java + Volley + HighCharts)**  
- **Home Screen**: Shows weather for the current location  
- **Search with Auto-complete** (Google Places API)  
- **Detailed Weather View**: Includes **Today’s conditions, Weekly Forecast, and Weather Data Charts**  
- **Favorites Management**: Add/remove locations (synced with MongoDB)  
- **Material UI, Ripple Effects, Floating Action Buttons, and Splash Screen**  

---

## **How to Run**  

### **1. Web App**  
**Live Demo:** [Weather Search](https://weather-search-project.wl.r.appspot.com/)  

To run locally:  
```bash
git clone https://github.com/your-repo/weather-app.git
cd weather-app/frontend
npm install
ng serve
```
Access the app at `http://localhost:4200/`  

### **2. Backend (Node.js + Express + MongoDB)**  
The backend is deployed on **Google Cloud App Engine**. To run locally:  
```bash
cd weather-app/backend
npm install
node server.js
```
Test API locally:  
```
http://localhost:5000/get_weather?city=Los+Angeles&state=CA
```

### **3. Android App**  
📱 **Demo Video Uploaded** (Refer to the repository)  
To run on an emulator:  
1. Open **Android Studio**  
2. Clone the repository  
3. Build & run the app on a **Pixel 5 emulator (Android 15)**  

---

## **Backend API Reference**  
Base URL:  
```
https://backend-dot-weather-search-project.wl.r.appspot.com/
```

### **Weather Data API**  
Fetches weather details using Tomorrow.io API.  
#### **Example Request:**  
```
https://backend-dot-weather-search-project.wl.r.appspot.com/get_weather?city=Los+Angeles&state=CA
```
#### **Response Format (JSON)**  
```json
{
  "location": "Los Angeles, CA",
  "temperature": 72,
  "weather": "Sunny",
  "humidity": 45,
  "windSpeed": 5,
  "forecast": [
    {"day": "Monday", "high": 75, "low": 60},
    {"day": "Tuesday", "high": 78, "low": 62}
  ]
}
```

---

## **Key Takeaways**  
🔹 **Cross-Platform Development**: Web & mobile apps use a shared **Node.js backend**  
🔹 **Cloud-Based Storage**: **MongoDB Atlas** ensures user preferences sync across devices  
🔹 **Advanced Visualizations**: **HighCharts** enhances data presentation  
🔹 **Scalable Deployment**: Hosted on **Google Cloud App Engine**  

---

## **Future Improvements**  
🚀 **Expand to iOS using Flutter/Kotlin Multiplatform**  
🚀 **Add Push Notifications for weather alerts**  
🚀 **Improve UI with Material Design 3**  

---

## **Contact**  
For any issues or improvements, feel free to open an **issue** or submit a **pull request**! 🚀  
