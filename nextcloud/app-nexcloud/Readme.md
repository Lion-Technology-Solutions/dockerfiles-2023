Using the apache image
The apache image contains a webserver and exposes port 80. To start the container type:

$ docker run -d -p 8080:80 nextcloud
#Now you can access Nextcloud at http://localhost:8080/ from your host system.
