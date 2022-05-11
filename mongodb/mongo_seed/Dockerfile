FROM mongo:latest
COPY apples.json /apples.json
COPY oranges.json /oranges.json
CMD mongoimport --host mongodb --db fruit --username root --password password --authenticationDatabase admin --collection apples --drop --type json --file /apples.json --jsonArray && \
    mongoimport --host mongodb --db fruit --username root --password password --authenticationDatabase admin --collection oranges --drop --type json --file /oranges.json --jsonArray