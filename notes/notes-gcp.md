## Google Cloud Setup

**Google Cloud SDK Installation**
- Follow the instructions on this link: https://cloud.google.com/sdk/docs/install
- CLI guide: https://cloud.google.com/sdk/gcloud

**Compute Instance VM**:
- NAME: advalen09-de-zoomcamp-vm
- ZONE: us-central1-a
- MACHINE_TYPE: t2a-standard-8
- INTERNAL_IP: 10.128.0.2
- EXTERNAL_IP: 34.135.29.24 (static)

**SSH to Virtual Machine using SDK**
- Open Google Cloud SDK
- Run:

```
gcloud init
gcloud compute ssh advalen09-de-zoomcamp-vm --project=advalen-de-zoomcamp-2024 --zone=us-central1-a
```

