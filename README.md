# File-Transfer-Application
This Java project creates a simple file transfer system. Clients can upload files to a server using a GUI. The server receives and processes uploads in real time, updating the client on progress. It demonstrates socket programming, multithreading, and GUI development in Java.

## Features

- **Client-Server Architecture**: Communication over sockets.
- **File Upload**: Clients can upload files of any size to the server.
- **Progress Tracking**: Real-time monitoring of file upload progress.
- **Multi-threading**: Server can handle multiple client connections simultaneously.
- **Graphical Interface**: Swing-based UI for file selection and upload on the client side.
```
## Folder Structure
├───classes
│       FileModel.class
│       FileUploadEvent.class
│       FileUploadListener.class
│       FileUploadThread.class
│       FTClientFrame$FileSelectionPanel.class
│       FTClientFrame$FileUploadViewPanel$ProgressPanel.class
│       FTClientFrame$FileUploadViewPanel.class
│       FTClientFrame.class
│       FTServer$1.class
│       FTServer.class
│       FTServerFrame.class
│       RequestProcessor$1.class
│       RequestProcessor.class
│
├───src
│       ftclient5.java
│       ftserver5.java
│
└───uploads
```
- **classes/**: Contains compiled Java class files for both the client and server.
- **src/**: Source code files (`ftclient5.java`, `ftserver5.java`) for the client-server application.
- **uploads/**: The folder where uploaded files are stored on the server.

## Getting Started

### Prerequisites

- Java Development Kit (JDK 8 or higher)

### Running the Server

1. Navigate to the project directory.
2. Compile the server code:
   ```bash
   javac -d classes src/ftserver5.java
   ```
### Running the Server
1. Run the server:
   ```bash
   java -classpath classes;. FTServerFrame
   ```
### Running the Client
1. Navigate to the project directory.
2. Compile the client code:
```bash
javac -d classes src/ftclient5.java
```
3. Run the client:
```bash
java -classpath classes;. FTClientFrame
```
### How it Works
1. Start the server on the designated port (default is 5500).
2. Run the client, which opens a graphical interface.
3. Use the client to select files for upload.
4. Monitor the progress of the upload in real time through the UI.
5. The server saves uploaded files to the uploads/ directory.

### Contributions
Feel free to fork the project, create issues, or submit pull requests to enhance the file transfer system.

### License
This project is licensed under the MIT License - see the LICENSE file for details.
