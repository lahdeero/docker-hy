FROM java
RUN mkdir /Lukuvinkki-NESMM
# muista ajaa "gradle build" lokaalisti
COPY ./Lukuvinkki-NESMM/build/libs/lukuvinkki-applikaatio.jar /Lukuvinkki-NESMM
WORKDIR /Lukuvinkki-NESMM
ENTRYPOINT java -jar lukuvinkki-applikaatio.jar
