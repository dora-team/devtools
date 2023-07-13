# Cloud Workstations Config
This folder contains configurations for working with Google Cloud Workstations.

The GCP project `doradotdev` hosts a [Workstations cluster](https://console.cloud.google.com/workstations/overview?project=doradotdev) that we can use. In this folder, we can host configs like Dockerfiles for custom workstation images. [Here's some documentation](https://cloud.google.com/workstations/docs/customize-container-images) about that.

TODO: #2 per those docs, we should "set up a [secure pipeline](https://cloud.google.com/software-supply-chain-security/docs/create-secure-image-pipeline) to automatically rebuild these images when the Cloud Workstations base image is updated"

### Helpful info
Here's the command(s) to connect a machine to Dave's workstation, so local VS Code can use it:
```sh
# start workstation and establish tcp tunnel
WORKSTATION_ID=stanke-20230517 \
gcloud beta workstations start \
--project=doradotdev \
--region=us-east4 \
--cluster=dora-team-devboxes \
--config=hugo-devboxes \
${WORKSTATION_ID} && \
gcloud beta workstations start-tcp-tunnel \
  --project=doradotdev \
  --region=us-east4 \
  --cluster=dora-team-devboxes \
  --config=hugo-devboxes \
  --local-host-port=:54321 \
  ${WORKSTATION_ID} 22
```
then, in VSCode, click the Remote Window widget, choose "connect [Current Window] to Host", and enter `user@localhost:54321`
