# docker-jclouds-cli

Docker image with jclouds cli

    docker run -ti --rm csanchez/jclouds-cli

    docker run -ti --rm \
      -e JCLOUDS_BLOBSTORE_IDENTITY="${AWS_ACCESS_KEY_ID}" \
      -e JCLOUDS_BLOBSTORE_CREDENTIAL="${AWS_SECRET_ACCESS_KEY}" \
      csanchez/jclouds-cli jclouds blobstore list --provider aws-s3 bucket_name
