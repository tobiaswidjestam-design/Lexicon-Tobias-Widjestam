# Installation – Software Developer, Java Group 63

This is where I document the software I installed on my computer as part of the
course's installation assignment.

## Installed software

| Software           | Version             | Purpose                                      |
| ------------------ | ------------------- | -------------------------------------------- |
| Git                | 2.55.0.windows.5    | Version control                              |
| JDK (Java)         | 21.0.12.1 (`javac`) | Compile and run Java programs                |
| IntelliJ IDEA      | 2026.1              | Integrated development environment (IDE)     |
| Visual Studio Code | Installed           | Code editor                                  |
| MySQL              | Installed           | Database                                     |
| Docker Desktop     | Installed           | Container environment                        |
| Node.js            | Installed           | JavaScript runtime (when needed)             |
| Maven              | 3.9.16              | Build tool / project management for Java (JavaFX) |

## Verifying the installations

Commands I used to check that the software works:

```bash
git --version      # git version 2.55.0.windows.5
javac -version     # javac 21.0.12.1
mvn -version       # Apache Maven 3.9.16, running on JDK 21 via JAVA_HOME
```

## Git configuration

```bash
git config --global user.name   # Aphex
git config --global user.email  # tobias.widjestam@gmail.com
```

## Notes

- `java -version` reported Java 8 (1.8.0_503) while `javac` is JDK 21 –
  PATH/JAVA_HOME needs to be configured so that `java` points to JDK 21.
- **Maven 3.9.16 is now installed** at `C:\Users\Administrator\apache-maven-3.9.16`
  and added to PATH. `mvn -version` confirms that Maven runs on JDK 21 (via JAVA_HOME).
- JavaFX 21 has been tested with a Maven project (`hellofx`): `mvn package` and
  `mvn javafx:run` both work. Maven downloads the JavaFX libraries automatically
  from `pom.xml` – no manual SDK needed.
