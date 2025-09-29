# keycloak-iam-project
A hands-on project to set up a local IAM server using Keycloak and Docker.
Project Summary
This project demonstrates the setup and configuration of a local Identity and Access Management (IAM) server using Keycloak, containerized with Docker. The primary goal was to build a hands-on understanding of core IAM concepts by creating a complete authentication flow for a sample web application, including realm and client configuration, user creation, and testing the end-to-end OpenID Connect (OIDC) login process.

Technologies Used
Keycloak: Open-source Identity and Access Management solution.

Docker: Containerization platform used to run the Keycloak instance locally.

PowerShell (Windows Terminal): Used to execute Docker commands and manage the container.

Key Features Implemented
Dockerized Keycloak Instance: Deployed a Keycloak server in a development environment using a single Docker command.

Realm and Client Configuration: Created an isolated realm (my-test-app) and registered a client application (my-web-app) with specific security settings, including a valid redirect URI.

User Management: Programmatically created a test user (testuser) and managed their credentials within the custom realm.

End-to-End Authentication Flow: Successfully tested the complete OIDC Authorization Code Flow, from user login to a successful redirect after authentication.

How to Run This Setup
Ensure Docker is installed. You can verify your installation with docker --version.

Run the Keycloak container using the following command in your terminal:

Bash

docker run -p 8080:8080 -e KEYCLOAK_ADMIN=admin -e KEYCLOAK_ADMIN_PASSWORD=admin quay.io/keycloak/keycloak:latest start-dev
Access the Admin Console by navigating to http://localhost:8080/ in your browser and logging in with admin / admin.

Follow the configuration steps outlined in the full project report PDF file to set up the realm, client, and user.

Project Conclusion
This project provided valuable, hands-on experience in deploying and managing a modern IAM solution. It successfully covered the fundamental steps of securing an application, from initial server setup to a complete, working user authentication flow. The process highlighted the power of containerization for creating reproducible development environments and solidified my understanding of the OIDC protocol.
