## Step 1

Open a terminal window in the same directory where the `Dockerfile` from this repository is located. Build the Jenkins Docker image:

```
docker build -t my-jenkins .
```

## Step 2

Start Jenkins:

```
docker compose up -d
```

## Step 3

Open Jenkins by going to: [http://localhost:8080/](http://localhost:8080/) and finish the installation process.

## Step 4

If you wish to stop Jenkins and get back to it later, run:

```
docker compose down
```

If you wish to start Jenkins again later, just run the same comand from Step 3.


# Removing Jenkins

Once you are done playing with Jenkins maybe it is time to clean things up.

Run the following comand to terminate Jenkins and to remove all volumes and images used:

```
docker compose down --volumes --rmi all 