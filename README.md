# FitBuddy

FitBuddy is a FastAPI web application that creates a general 7-day fitness plan, stores users/plans in SQLite, and optionally uses Google Gemini for generation and plan updates.

## VS Code setup
1. Extract this folder and open `FitBuddy` in VS Code.
2. Open a terminal.
3. Create a virtual environment:
   - Windows: `python -m venv venv` then `venv\\Scripts\\activate`
   - macOS/Linux: `python3 -m venv venv` then `source venv/bin/activate`
4. Install dependencies: `pip install -r requirements.txt`
5. Copy `.env.example` to `.env`.
6. Add `GEMINI_API_KEY` if you want Gemini; without it the app uses safe demo fallback content.
7. Run: `python -m uvicorn app.main:app --reload`
8. Open `http://127.0.0.1:8000`.

## API docs
Open `/docs` for Swagger UI and `/redoc` for ReDoc.

## Tests
Run `python -m pytest -q`.

## Admin page
Open `/view-all-users`. Set `ADMIN_KEY` in `.env` to protect it.
