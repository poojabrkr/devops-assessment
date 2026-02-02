FROM python:3.10-slim AS base

RUN useradd -m appuser
WORKDIR /app

COPY requirements.txt.
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

USER appuser
EXPOSE 8000

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]

