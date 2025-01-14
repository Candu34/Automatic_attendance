# Automatic Attendance

A Java-based application designed for efficient and automated attendance tracking. This project uses Docker Compose to manage its environment and supports development in IntelliJ IDEA.

---

## Prerequisites

Before setting up the project, ensure the following tools are installed:

1. [IntelliJ IDEA](https://www.jetbrains.com/idea/download/)
2. [Docker Desktop](https://www.docker.com/products/docker-desktop)

---

## Setup and Installation

### 1. Install IntelliJ IDEA
- Download IntelliJ IDEA Community or Ultimate from [JetBrains](https://www.jetbrains.com/idea/download/).
- Follow the installation steps for your OS.
- Open IntelliJ and set up the Java JDK if prompted.

### 2. Install Docker Desktop
- Download Docker Desktop from [Docker](https://www.docker.com/products/docker-desktop).
- Install and start Docker Desktop. Ensure Docker is running before proceeding.

### 3. Clone the Repository
Clone this repository using the command below:
```bash
git clone https://github.com/Candu34/Automatic_attendance.git
cd Automatic_attendance
```

### 4. Open the Project in IntelliJ IDEA
1. Launch IntelliJ IDEA.
2. Select **File > Open** and navigate to the project folder.
3. IntelliJ will detect the Maven or Gradle structure and import the project dependencies.

### 5. Start Docker Containers
1. Open the **Docker** tab in IntelliJ (available in the toolbar).
2. Locate the `docker-compose.yml` file in the project directory.
3. Right-click on the file and select **Run 'docker-compose up'** to start the containers.

### 6. Verify the Database Connection
1. Open the **Database** tab in IntelliJ IDEA (use **View > Tool Windows > Database** if it's not visible).
2. Click the **+** icon and select **Data Source > PostgreSQL** (or the database you are using).
3. Fill in the connection details as specified in `docker-compose.yml`:
   - Host: `localhost`
   - Port: `<Database Port>`
   - Database: `<Database Name>`
   - Username: `<DB Username>`
   - Password: `<DB Password>`
4. Test the connection and save it.

### 7. Run the Application
1. Ensure that all Docker containers are running.
2. Use IntelliJ's **Run/Debug Configuration** to start the application.
3. Access the application via the specified URL in your browser or API testing tool.

---

## Application Features

1. **Automated Attendance Tracking**
2. **User-Friendly Interface**
3. **Database Integration with Docker**
4. **Customizable Configuration**

---

## Troubleshooting

- If Docker fails to start, verify that Docker Desktop is running and restart IntelliJ IDEA.
- Ensure all required ports in `docker-compose.yml` are available and not in use by other services.
- Check for dependency conflicts in the `pom.xml` or `build.gradle` file.

---

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

---

## License

This project is licensed under the MIT License.

