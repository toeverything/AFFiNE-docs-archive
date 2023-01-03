# 🆒 Install AFFiNE with Docker

! Please note that the current Docker deploys the pre-alpha version. We are still working on creating a Docker image for the newer alpha version, please bear with us.

This guide assumes you already have an environment setup running docker.

Currently there are two main versions:
1) AFFiNE - you are looking at running AFFiNE locally first.
2) AFFiNE (with server-side support) - you are looking for enhanced server-side functionality, such as collaboration and server-side storage.

### Installing AFFiNE using Docker

* Pull the latest AFFiNE image. This may take some time depending on your network connection.

```
docker pull ghcr.io/toeverything/affine:nightly-latest
```

Ensure this step is completed successfully before continuing (you can rerun this command if you are unsure).

* Next we will run the AFFiNE project in Docker.

```
docker run -p 4200:3000 --name affine -d ghcr.io/toeverything/affine:nightly-latest
```

This command binds the internal app port 3000 to the public port 4200.

* You can confirm that AFFiNE is running successfully by using the command

```
docker ps
```

This command shows a list of running containers - in the list you should be able to find AFFiNE.

* Now you can access AFFiNE from your browser via:
  * If you are running Docker on your local machine and using the default settings you can access via port 4200 through localhost: [http://localhost:4200/](http://localhost:4200/)
  * Otherwise you will need to know the {IP} of the machine using Docker and the {PORT} that AFFiNE is using.

### Installing AFFiNE (with server-side support) using Docker

* Pull the latest AFFiNE image. This may take some time depending on your network connection.

```
docker pull ghcr.io/toeverything/affine:nightly-server-latest
```

Ensure this step is completed successfully before continuing (you can rerun this command if you are unsure).

* Next we will run the AFFiNE project in Docker.

```
docker run -it --rm -p 3000:3000 ghcr.io/toeverything/affine:nightly-server-latest
```

This command binds the internal app port 3000 to the public port 3000. You should also change You can also add a flag to bind the Docker volume that is used for data storage with the ```-v``` flag ```docker run -it --rm -p 3000:3000 -v YOUR_PATH:/app/data ghcr.io/toeverything/affine:nightly-server-latest```. Don't forget to replace ```YOUR_PATH```.

* You can confirm that AFFiNE is running successfully by using the command

```
docker ps
```

This command shows a list of running containers - in the list you should be able to find AFFiNE.

* Now you can access AFFiNE from your browser via:
  * If you are running Docker on your local machine and using the default settings you can access via port 3000 through localhost: [http://localhost:3000/](http://localhost:3000/)
  * Otherwise you will need to know the {IP} of the machine using Docker and the {PORT} that AFFiNE is using.
