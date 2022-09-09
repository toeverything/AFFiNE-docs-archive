# 🆒 Install AFFiNE with Docker

This guide assumes you already have an environment setup running docker.

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
