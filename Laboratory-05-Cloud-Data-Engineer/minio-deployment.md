# MinIO Deployment Documentation
## Docker Command Used
```bash
docker run -d \
  -p 9000:9000 \
  -p 9001:9001 \
  --name minio-server \
  -e "MINIO_ROOT_USER=cloudadmin" \
  -e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
  quay.io/minio/minio server /data --console-address ":9001"
```

## Web Console Port
The MinIO Web Console was accessed using port 9001.
Bucket Created
* Bucket Name: client-photos
## Explanation of the -e Flags (Environment Variables)
The -e flags are used to set environment variables inside the Docker container when it starts.
* MINIO_ROOT_USER=cloudadmin
This sets the administrator username for logging into the MinIO console.
* MINIO_ROOT_PASSWORD=CloudNova2026
This sets the administrator password, also These environment variables ensure secure access to the MinIO server by defining custom credentials instead of using defaults.
