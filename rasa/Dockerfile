FROM rasa/rasa:3.4.0-full
USER root

WORKDIR /app

COPY . .

RUN rasa train --domain domain.yml --data data --out models --force

ENTRYPOINT [ "rasa" ]

CMD [ "run", "--enalble-api", "--cors", '"*"' ]
