
FROM python:3.7
WORKDIR /app
COPY . /app
RUN pip install -r api_yamdb/requirements.txt --no-cache-dir
CMD ["gunicorn", "api_yamdb.wsgi:application", "--bind", "0:8000" ]