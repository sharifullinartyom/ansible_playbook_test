FROM maven:3.9-eclipse-temurin-21

WORKDIR /app

COPY . .

RUN mvn clean package -DskipTests

CMD ["sh", "-c", "mkdir -p /app/dist && cp target/*.war /app/dist/ROOT.war"]