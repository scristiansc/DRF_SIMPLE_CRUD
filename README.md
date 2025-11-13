# 🧩 CRUD API with Django Rest Framework

This project is a **REST CRUD API** built with **Django Rest Framework (DRF)**. It allows creating, reading, updating, and deleting projects.

It is deployed on Render and includes **interactive documentation** via Swagger and Redoc.

---

## 🚀 Technologies Used

- Python 3.x
- Django
- Django Rest Framework
- drf-spectacular (Swagger / Redoc)
- SQLite (local) / PostgreSQL (production)
- Deployment on Render

---

## 📦 Local Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/your-repo.git
cd your-repo

2. Create and activate a virtual environment:

python -m venv venv
# Windows
venv\Scripts\activate
# Mac/Linux
source venv/bin/activate

3. Install dependencies:

pip install -r requirements.txt

4. Apply migrations:

python manage.py migrate

5. Run the server:

python manage.py runserver

6. Access the API in your browser:

http://127.0.0.1:8000/

🔗 Endpoints
API Root
GET /
Returns the main available resources:

json
Copiar código
{
    "api/projects": "http://127.0.0.1:8000/api/projects/"
}

Projects CRUD
Base URL: /api/projects/

HTTP Method	Endpoint	Description	Example Payload (JSON)
GET	/api/projects/	List all projects	-
POST	/api/projects/	Create a new project	{ "name": "Project A", "description": "Description" }
GET	/api/projects/{id}/	Get a specific project	-
PUT	/api/projects/{id}/	Replace a project completely	{ "name": "New name", "description": "New description" }
PATCH	/api/projects/{id}/	Partially update a project	{ "description": "Partial update" }
DELETE	/api/projects/{id}/	Delete a project

📖 Interactive Documentation

Documentation is automatically generated using drf-spectacular:

Swagger UI:
http://127.0.0.1:8000/api/docs/

Redoc:
http://127.0.0.1:8000/api/redoc/

You can test all endpoints live, see descriptions, and example request/response from these pages.

🛠 Production Usage

If deployed on Render:

API Root: https://drf-simple-crud-qz8l.onrender.com/

Projects Endpoint: https://drf-simple-crud-qz8l.onrender.com/api/projects/

Swagger UI: https://drf-simple-crud-qz8l.onrender.com/api/docs/

🧾 License

This project is distributed under the MIT License.