# File Management API with Spring Boot

This is a simple Java Spring Boot API for file management. It allows you to upload files, download files, and list all available files.

## Getting Started

Follow the instructions below to use this API for file management.

### Prerequisites

Before you begin, ensure you have the following installed:

- Java Development Kit (JDK)
- Maven
- curl (for testing)

### Running the API

1. Clone this repository:
   ```shell
   git clone https://github.com/yourusername/your-api-repo.git

2. Navigate to the project directory:
    ```
    cd your-api-repo

3. Build and run the Spring boot application:
    ```
    mvn spring-boot:run
The api will start running on `https://localhost:8080`

## Usage
### Uploading a file
To upload a file, use the following `curl` command:

    
    curl -X POST -F "file=@/path/to/your/file.jpg" http://localhost:8080/api/file/upload

Replace `/path/to/your/file` with the path to the file you want to upload

### Downloading file
To download a file, use the following `curl` command:

    curl -OJL https://localhost:8080/api/files/download/filename.jpg -v
replace `filename.jpg` with the name of the file you want to download

### Listing all files
To list all the files available on the server, use the following `curl` command:

    curl http://localhost:8080/api/files/list

