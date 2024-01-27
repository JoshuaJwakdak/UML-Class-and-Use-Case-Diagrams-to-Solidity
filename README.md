# UML-Class-and-Use-Case-Diagrams-to-Solidity
UML Class and Use-Case Diagrams to Solidity
This app takes in Class and Use-Case XML files as input and coverts them to solidity code as well as display the UML diagram.
This app is a docker image as such, you have to run it in a docker container.


**Additional Steps for X Server Support:**

1.  Install X Server: https://sourceforge.net/projects/vcxsrv/
Before running the Docker container, ensure that you have an X server installed on your machine. 
For Windows, you can use Xming or VcXsrv. For Linux, you can use the default X server.

2.  Configure X Server:
Start your X server (e.g., Xming or VcXsrv) before running the Docker container. 
Make sure it is configured to allow connections from localhost.

**Installation Instructions for UML-to-Solidity Docker Image**

1.  Install Docker: https://www.docker.com/products/docker-desktop/
Make sure Docker is installed on your machine. If not, 
download and install Docker from the official website: Docker Desktop.

2.  Download UML-to-Solidity Docker Image:D
Download the Docker image tarball (uml_to_solidity.tar) provided.

3.  Load Docker Image:
Open a terminal or command prompt and navigate to the directory containing the downloaded tarball.
Run the following command to load the Docker image:

bash

        docker load -i uml_to_solidity.tar

4. Run Docker Container:

After loading the image, run the Docker container with the following command:

bash

        docker run -it uml-to-sol3:latest

5. Replace uml-to-sol3:latest with the correct image name and tag obtained from the output of the docker images command.

6. Use the UML-to-Solidity Application:
Once inside the Docker container, you can use the UML-to-Solidity application by running the image.

7. Exit the Docker Container:
When finished, exit the Docker container by typing exit in the terminal.


Ensure Docker is running on your machine before attempting to load and run the Docker image.
Make sure to use the correct image name and tag when running the container.
  

**Note**

All the Xml files for testing is found in the docker container, 
when you run the app and after you have selected the option of which uml diagram to convert, 
a button appears which is browse file, it then  displays     the list of xml files. 
make sure to select appropraite xml file according to your initial option choice. 
They are categorized into class and use-case diagrams accordingly.
