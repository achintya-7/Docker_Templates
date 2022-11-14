FROM python

WORKDIR /app

COPY ./requirements.txt .

RUN pip install -r requirements.txt

COPY . .

# Or whatever port you want to expose
EXPOSE 8000

CMD ["uvicorn",  "app.main:app", "--host=0.0.0.0", "--reload"]