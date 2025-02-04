Number Classification API 🚀

Overview

This API classifies numbers based on mathematical properties and provides fun facts.
Features

✔ Check if a number is Prime, Armstrong, or Perfect
✔ Fetch fun facts from Numbers API
✔ Handles CORS for external access
✔ Fast response time (<500ms)

🚀 How to Use

Base URL
https://web-production-3144.up.railway.app
API Endpoint
GET /api/classify-number?number={number}
Example Request
GET /api/classify-number?number=371

Example Response
{
    "number": 371,
    "is_prime": false,
    "is_perfect": false,
    "properties": ["armstrong", "odd"],
    "digit_sum": 11,
    "fun_fact": "371 is an Armstrong number because 3^3 + 7^3 + 1^3 = 371"
}

⚙️ Local Setup

1️⃣ Clone the Repository
git clone https://github.com/Temitopeade23/number-classification-api.git
cd number-classification-api
2️⃣ Create and Activate a Virtual Environment
python -m venv venv
source venv/bin/activate  # On Mac/Linux
venv\Scripts\activate     # On Windows
3️⃣ Install Dependencies
pip install -r requirements.txt
4️⃣ Run the API Locally
python app.py
or using Flask CLI:
flask run --host=0.0.0.0 --port=5000
5️⃣ Test Locally
Open your browser and visit:
http://127.0.0.1:5000/api/classify-number?number=371

🌍 Live API

The API is deployed on Railway and can be accessed at:
https://web-production-3144.up.railway.app/api/classify-number?number=371
📂 Project Structure

number-classification-api/
│── app.py             # Flask app logic
│── requirements.txt   # Dependencies
│── Procfile           # Railway deployment instructions
│── README.md          # Project documentation
📜 License

This project is open-source and available under the MIT License.
