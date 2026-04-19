# Gender Classifier API - Stage 0

A lightweight Node.js service that integrates with the Genderize.io API to predict the gender of a name with added confidence logic and structured data processing.

## 🚀 Live Endpoint
[INSERT_YOUR_VERCEL_URL_HERE]/api/classify?name=john

## 🛠 Tech Stack
- **Runtime:** Node.js
- **Framework:** Express.js
- **HTTP Client:** Axios
- **Deployment:** Vercel

## 📌 API Specification

### Classify Name
Returns gender prediction and confidence metrics for a given name.

**GET** `/api/classify?name={name}`

**Success Response (200 OK):**
```json
 {
   "status": "success",
   "data": {
     "name": "john",
     "gender": "male",
     "probability": 0.99,
     "sample_size": 1234,
     "is_confident": true,
     "processed_at": "2026-04-01T12:00:00Z"
   }
 }
