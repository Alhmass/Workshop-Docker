FROM openjdk:11-slim-buster as builder
LABEL MAINTENER="hugo.lumet@epitech.eu"
RUN apt-get update && apt-get install -y \
  git \
  && rm -rf /var/lib/apt/lists/*
RUN mkdir -p /src/app/
WORKDIR /src/app/
COPY . /src/app/
RUN java -jar BuildTools.jar --rev 1.14.2

FROM openjdk:11-jre-slim
LABEL MAINTENER="hugo.lumet@epitech.eu"
RUN mkdir -p /src/app/ \
  && groupadd -r mcgroup \
  && useradd -r -s /bin/false -g mcgroup mcuser \
  && chown -R mcuser:mcgroup /src/app/
WORKDIR /src/app
COPY --from=builder /src/app/spigot-1.14.2.jar /src/app/
EXPOSE 25565
USER mcuser
RUN echo eula=true >> eula.txt
CMD ["java", "-jar", "spigot-1.14.2.jar"]