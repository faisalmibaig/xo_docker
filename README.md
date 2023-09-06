# Xen Orchestra Docker Image

**Build Instructions:**

Clone the repository and navigate into the "build_files" folder. Run `docker build . -t local/xo:1.0` to build your Xen Orchestra image.

Once the build is complete, generate self-signed certificates in the "config" folder.
`openssl req -x509 -newkey rsa:4096 -keyout orchestra_key.pem -out orchestra_cert.pem -days 3650 -nodes -subj '/CN=orchestra.local'`

Default Credentials to the web UI:
user: admin@admin.net
password: admin

**Disclaimer: Data is not persistant and all data will be lost on container reboot**
