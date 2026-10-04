# main.py
from fastapi import FastAPI

app = FastAPI(
    title="Transport AI API",
    description="AI-powered transport disruption information and passenger assistance platform.",
    version="0.1.0",
)


@app.get("/")
def read_root():
    return {
        "message": "Transport AI Disruption Platform API running",
        "status": "online",
    }