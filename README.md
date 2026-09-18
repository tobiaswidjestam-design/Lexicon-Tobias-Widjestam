# Installation – Software Developer, Java Group 63

Här dokumenterar jag de program jag installerat på min dator som en del av
kursens installationsuppgift.

## Installerade program

| Program            | Version                  | Syfte                                |
| ------------------ | ------------------------ | ------------------------------------ |
| Git                | 2.55.0.windows.5         | Versionshantering                    |
| JDK (Java)         | 21.0.12.1 (`javac`)      | Kompilera och köra Java-program      |
| IntelliJ IDEA      | 2026.1                   | Utvecklingsmiljö (IDE)               |
| Visual Studio Code | Installerad              | Kodredigerare                        |
| MySQL              | Installerad              | Databas                              |
| Docker Desktop     | Installerad              | Containermiljö                       |
| Node.js            | Installerad              | JavaScript-runtime (vid behov)       |
| Maven              | 3.9.16                   | Byggverktyg/projekthantering för Java (JavaFX) |

## Verifiering av installationerna

Kommandon jag använt för att kontrollera att programmen fungerar:

```bash
git --version      # git version 2.55.0.windows.5
javac -version     # javac 21.0.12.1
mvn -version       # Apache Maven 3.9.16, kör på JDK 21 via JAVA_HOME
```

## Konfiguration av Git

```bash
git config --global user.name   # Aphex
git config --global user.email  # tobias.widjestam@gmail.com
```

## Noteringar

- `java -version` rapporterade Java 8 (1.8.0_503) medan `javac` är JDK 21 –
  PATH/JAVA_HOME behöver ställas in så att `java` pekar på JDK 21.
- **Maven 3.9.16 är nu installerat** på `C:\Users\Administrator\apache-maven-3.9.16`
  och lagt på PATH. `mvn -version` bekräftar att Maven kör på JDK 21 (via JAVA_HOME).
- JavaFX 21 har testats via ett Maven-projekt (`hellofx`): `mvn package` och
  `mvn javafx:run` fungerar. Maven laddar JavaFX-biblioteken automatiskt från
  `pom.xml` – ingen manuell SDK behövs.
