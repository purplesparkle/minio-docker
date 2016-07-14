# About this Repo


# Build
```sh
docker build .
```

# Run
```sh
docker run -d -v /data/disk1:/minio/data -v /data/config:/minio/config -p 9000:9000 -e MINIO_ACCESS_KEY=remco -e MINIO_SECRET_KEY=remcoremco d4b3
```

## Volumes
/minio/data volume containing the data
/minio/config volume containing config

## Parameters

MINIO_ACCESS_KEY: predefined access key (min 5 chars)
MINIO_SECRET_KEY: predefined secret key
```sh
docker run -d -v /data/disk1:/minio/data -v /data/config:/minio/config -p 9000:9000 -e MINIO_ACCESS_KEY=remco -e MINIO_SECRET_KEY=remcoremco d4b3
```

MINIO_CACHE_SIZE: defaults to 8g
MINIO_CACHE_EXPIRY: defaults to 72h
