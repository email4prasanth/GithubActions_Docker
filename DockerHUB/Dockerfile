FROM python:3.12-slim
LABEL author="prasanth"
WORKDIR /app
COPY ./DockerHUB/requirements.txt /app/
RUN pip install --no-cache-dir -r requirements.txt
CMD ["python", "app.py"]

