# MadarsaHub: Oracle server try

GitHub tries every 15 minutes to make the free Oracle ARM server (`madarsahub-server`: Ubuntu 24.04, 2 CPU / 12 GB,
or 1 CPU / 6 GB if the bigger one has no room). When the server exists, the workflow switches itself off.

Secrets (Settings -> Secrets and variables -> Actions):

| Name | Value |
| --- | --- |
| `OCI_USER` | `user=` line from Oracle's API key "Configuration file preview" |
| `OCI_FINGERPRINT` | `fingerprint=` line |
| `OCI_TENANCY` | `tenancy=` line |
| `OCI_REGION` | `ap-osaka-1` |
| `OCI_KEY` | the whole downloaded API private key file (`-----BEGIN PRIVATE KEY-----` ... `END PRIVATE KEY-----`) |
| `SSH_PUBLIC_KEY` | the whole `.pub` file of the server's SSH key (one line, `ssh-rsa ...`) |
