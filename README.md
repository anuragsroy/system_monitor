"# system_monitor" 
<img width="561" height="191" alt="Untitled Diagram drawio" src="https://github.com/user-attachments/assets/9ccff569-9fbd-484f-ab98-8cdb4151b0be" />

**Tech Stack Choices:**
1. The backend microservice was created using Python due to the readily available modules to execute a particular task.
2. The Frontend dashboard was created using the React framework due to the ease of use
3. Pipelines were created using Jenkins

**Local Deployment Guide**
1. Backend
    a. Install dependencies (For Python 3.8+, install fastapi and uvicorn)
    b. Run the server using the following command:
       uvicorn app:app --reload
         where first app = filename (app.py) and second app = FastAPI instance name. --reload auto-reloads server on code changes.
    c. Access the endpoint: Open in browser or use curl: http://127.0.0.1:8000/metrics

3. Frontend
    a. React Code:
          - Create a new react project
              npx create-react-app metrics-dashboard (npm required to be installed)
              cd metrics-dashboard
          - Install Chart.js & react-chartjs-2
               npm install chart.js react-chartjs-2
          - Replace src/App.js with the App.js present in https://github.com/anuragsroy/react-files-frontend.git
          - Add App.css for a simple UI design and feel. This file is also present in https://github.com/anuragsroy/react-files-frontend.git
          - We need to make sure the app.py backend service is running, and then run "npm start"
          - Accessible in http://localhost:3000.



         
