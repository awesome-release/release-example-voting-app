 image build information :

| **Item**              | **Description**                                |
| --------------------- | ---------------------------------------------- |
| **Base**              | `maven:3.5-jdk-8-alpine`                       |
| **Work directory**    | `/code`                                        |
| **Build instruction** | `mvn package -D skiptests`                     |
| **Ports**             | N/A                                            |
| **Runtime image**     | `openjdk:8-jre-alpine`                         |
| **Launch command**    | `java -jar target/worker-jar-dependencies.jar` |

