# neo4j-backup-gcs

Create a backup of a specified neo4j db to Google Cloud Storage

## Configuration

Set the following environment variables for the Docker container:

`NEO4J_HOST` Hostname of neo4j db

`NEO4J_PORT` Port of neo4j db

`GCS_BUCKET_NEO4J` Google Cloud Storage bucket name

`BACKUP_NAME` Name of the backup file, will be appended by the current date

`GOOGLE_APPLICATION_CREDENTIALS` Path to mounted credentials file (google service account key json file)

`PROTOCOL` The protocol to do the backup from. If not specified, then we use "catchup". Read more about protocols [here](https://neo4j.com/docs/operations-manual/3.5/backup/performing/)
