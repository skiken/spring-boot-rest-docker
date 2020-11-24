FROM java:8
VOLUME /tmp
ADD spring-boot-rest-mysql.jar app.jar
EXPOSE 8008
RUN sh -c 'touch /app.jar'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]
