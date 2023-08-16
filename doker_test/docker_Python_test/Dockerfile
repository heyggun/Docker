FROM python:3.10

WORKDIR /tmp
COPY main.py /tmp/main.py
RUN pip install fastapi[all]
EXPOSE 80
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "80"]
