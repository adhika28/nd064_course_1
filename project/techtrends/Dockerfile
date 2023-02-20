FROM python:3.8

COPY . /app2
WORKDIR /app2

RUN pip install --no-cache-dir -r requirements.txt

RUN python init_db.py

COPY . .

EXPOSE 3111

CMD [ "python", "app.py" ]

