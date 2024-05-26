# BookMarker
Your Personal Book Marker

## Project Description
This project is a personal bookmark where you can store your favorite websites.

## Prerequisites
- Git
- Docker
- Kubernetes (Minikube)
- `kubectl` command-line tool

## How to Run

### Cloning the Repository
```bash
$ git clone https://github.com/peng1z/BookMarker.git
$ cd BookMarker
```

### Running the Application Locally
To start:
```bash
$ ./run.sh start
```
To stop:
```bash
$ ./run.sh stop
```

### Managing Dependent Services
To start:
```bash
$ ./run.sh start_infra
```
To stop:
```bash
$ ./run.sh stop_infra
```

### Running on Kubernetes
Creating a Kubernetes Cluster with Kind:
```bash
$ cd BookMarker/kind
$ ./create-cluster.sh
```
Deploying the Application
```bash
$ cd ../
$ kubectl apply -f k8s/
```

### Accessing the Application
- API:
  - NodePort: http://localhost:18080/api/bookmarks
- UI:
  - NodePort: http://localhost:30080/

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements or suggestions.

For detailed instructions, refer to the official Kubernetes documentation.