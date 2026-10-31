AURORA AI BACKEND UPDATE

Extract this ZIP. Keep this folder structure when uploading to your GitHub repository:

repository-root/
  index.html                 (KEEP YOUR EXISTING FILE)
  render.yaml
  backend/
    __init__.py
    main.py
    requirements.txt

Do not upload the ZIP itself to the repository. Extract it and upload the files/folders.
Do not replace or delete index.html.

Render build command: pip install -r backend/requirements.txt
Render start command: uvicorn backend.main:app --host 0.0.0.0 --port $PORT

Set DATABASE_URL to your Supabase PostgreSQL Session Pooler connection URI.
Keep JWT_SECRET, AURORA_MODEL_BASE_URL, AURORA_MODEL_API_KEY and AURORA_MODEL_NAME configured in Render.
Never share DATABASE_URL or AURORA_MODEL_API_KEY publicly.
