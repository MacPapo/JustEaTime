## README

This README provides instructions on how to use `JustEaTime` to set up and run the project.

### Prerequisites
Before proceeding, make sure you have the following prerequisites installed on your system:
- Docker: [Install Docker](https://docs.docker.com/engine/install/)
- Docker Compose: [Install Docker Compose](https://docs.docker.com/compose/install/)

### Getting Started
To get started with the project, follow the steps below:

1. Clone the repository:
   ```shell
   git clone --recursive https://github.com/MacPapo/JustEaTime.git
   cd JustEaTime
   ```

2. Configure Environment Variables:
   - Rename the `.env.example` file to `.env`.
   - Open the `.env` file and update the necessary environment variables based on your configuration.

3. Build and Start the Containers:
   ```shell
   docker-compose up --build
   ```

   This command will build the Docker images and start the containers defined in the `docker-compose.yml` file.

4. Access the Application:
   Once the containers are up and running, you can access the application in your browser at `http://localhost:<port>`, where `<port>` is the specified port in the `.env` file or the default port if not specified.

### Additional Information
- To stop the running containers, you can use the following command:
  ```shell
  docker-compose down
  ```

- If you make changes to the project code or configuration files, you will need to rebuild the containers by running `docker-compose up --build` again.

- For more detailed information and customization options, please refer to the project's documentation or configuration files.

### Troubleshooting
If you encounter any issues during the setup or running of the project, you can try the following steps:
- Ensure that all prerequisites are correctly installed.
- Verify that the necessary ports specified in the `.env` file are not already in use.
- Check the project's documentation or seek support from the project's maintainers for further assistance.