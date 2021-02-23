FROM jinaai/jina:{{ jina_version }}

COPY . /workspace
WORKDIR /workspace

RUN apt-get update && pip install -r requirements.txt

RUN python app.py dryrun

ENTRYPOINT ["python", "app.py"]
