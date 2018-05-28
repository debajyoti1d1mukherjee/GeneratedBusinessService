FROM java:8-alpine
VOLUME /Balance
ADD Balance.jar app.jar
RUN sh -c 'touch app.jar'
EXPOSE 8260
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-Dspring.profiles.active=docker","-jar","/app.jar"]
