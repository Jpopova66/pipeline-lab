FROM python:3.14-slim

WORKDIR /app

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

ARG APP_VERSION=dev
ENV APP_VERSION=${APP_VERSION}

EXPOSE 8000
CMD ["python", "-m", "flask", "--app", "app", "run", "--host", "0.0.0.0", "--port", "8000"]
