
Country Population Lookup - README

This repository contains the Country Population Lookup application, built as part of the Software Engineers – Second Interview Assignment for Elanco. The application fetches country population data from a REST API and provides a clean, intuitive frontend for users to search and visualize data.

---

Features
- Search bar with autocomplete suggestions for country names.
- Dynamic widgets displaying country flags and populations.
- Interactive bar chart comparing populations of selected countries.
- Limit of 6 countries for better usability and clarity.

---

Technologies Used
- Frontend: React.js
- Backend: Flask (Python)
- Data Source: REST Countries API
- Styling: CSS (with a blue-white theme for better UX)

---

Prerequisites
Ensure the following software is installed on your system:
1. Python 3.7 or above
2. Node.js (v14 or above) with npm
3. Git for version control

---

Setup Instructions

Step 1: Clone the Repository
```bash
git clone https://github.com/owlyoungish349/elanco-project.git
cd elanco-project
```

---

Step 2: Set Up the Backend
1. Navigate to the `backend` directory:
   ```bash
   cd backend
   ```
2. Create and activate a virtual environment:
   - On Windows:
     ```bash
     python -m venv venv
     venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     python3 -m venv venv
     source venv/bin/activate
     ```
3. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Start the Flask backend:
   ```bash
   python app.py
   ```
   - The backend will start running at `http://127.0.0.1:5000`.

---

Step 3: Set Up the Frontend
1. Navigate to the `frontend` directory:
   ```bash
   cd ../frontend
   ```
2. Install the required dependencies:
   ```bash
   npm install
   ```
3. Start the React development server:
   ```bash
   npm run dev
   ```
   - The frontend will start running at `http://127.0.0.1:5173`.

---

Step 4: Test the Application
1. Open your browser and navigate to `http://127.0.0.1:5173`.
2. Use the search bar to look up country populations and view results in the widgets and bar chart.

---

Project Structure
```
elanco-project/
│
├── backend/
│   ├── app.py               # Flask backend API
│   ├── requirements.txt     # Backend dependencies
│   └── ...                  # Additional backend files
│
├── frontend/
│   ├── src/
│   │   ├── components/      # React components
│   │   ├── App.jsx          # Main application file
│   │   └── ...              # Other frontend files
│   ├── package.json         # Frontend dependencies
│   └── ...                  # Additional frontend files
│
├── README.md                # Project setup instructions
└── ...                      # Other project files
```

---

Common Issues
- Backend Errors:
  - Ensure the virtual environment is activated before running the backend.
  - Verify that Python and Flask are installed correctly.

- Frontend Errors:
  - Ensure `npm install` has been run successfully.
  - If port conflicts occur, stop any processes running on port 5173 and restart the frontend server.

- API Issues:
  - Confirm that the Flask backend is running at `http://127.0.0.1:5000`.
  - If the API key or base URL is outdated, update it in `app.py`.

---

Future Improvements
- Add live deployment to AWS/Azure.
- Integrate additional data points like GDP and area.
- Implement user authentication for personalization.

---

If you encounter any issues or have questions, feel free to reach out. Thank you for reviewing this project! 😊
