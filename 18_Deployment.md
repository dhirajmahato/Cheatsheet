## Deployment

**1. Docker**

usecases: 

Modernizing monolithic architecture through Docker containers helps with scalability and agility. By compartmentalizing complex systems into discrete, manageable modules, organizations can seamlessly transition to a microservices architecture. 

<img width="708" height="270" alt="image" src="https://github.com/user-attachments/assets/9768b949-2d93-4013-a779-457872b5fdb7" />

- **Dockerfiles** are collections of instructions that instruct you on creating a specific Docker image.
- **Docker Image** an image a blueprint or picture of what will be in a container when it is operational. Images include the application’s code, or binary, runtimes, libraries, and other filesystem items. 

You may manually generate images with a Dockerfile, which is a text document that contains all of the instructions needed to produce a Docker image. You can also use the command docker pull [name] to grab images from a central repository known as a registry or from repositories such as Docker Hub.
- **Docker Container**  is a running instance of a Docker image.
  
        Docker Image (Blueprint)
        -------------------------
        |  App Code            |
        |  Runtime (Python)    |
        |  Libraries           |
        |  OS-level files      |
        -------------------------
                 ↓
        docker run
                 ↓
        Docker Container (Running App)
        -------------------------------
        |  Running Process            |
        |  Isolated Environment       |
        |  Uses Host OS Kernel        |
        -------------------------------
