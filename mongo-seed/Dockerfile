FROM mongo

COPY gsections_data01.js /gsections_data01.js

#ADD start.sh /start.sh
#RUN chmod +x /start.sh

# CMD mongoimport --host mongodb --db exampleDb --collection contacts --type json --file /init.json --jsonArray
CMD mongoimport -u "username" -p "password" --authenticationDatabase "admin" -d "blog" -c "gsections" --type json --file "gsections_data01.js"
CMD mongo blog blog-add-user01.js -u "username" -p "password" --authenticationDatabase "admin"
