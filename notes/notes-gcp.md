## Google Cloud Setup

**Google Cloud SDK Installation**
- Follow the instructions on this link: https://cloud.google.com/sdk/docs/install
- CLI guide: https://cloud.google.com/sdk/gcloud

**Compute Instance VM**:
- NAME: xxxxxxx-de-zoomcamp-vm
- ZONE: us-central1-a
- MACHINE_TYPE: t2a-standard-8
- INTERNAL_IP: 10.xxx.x.x
- EXTERNAL_IP: 34.xxx.xx.xx (static)

**SSH to Virtual Machine using SDK**
- Open Google Cloud SDK
- Run:

```
gcloud init
gcloud compute ssh instancename --project=projectname --zone=us-central1-a
```

