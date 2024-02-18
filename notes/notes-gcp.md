## Google Cloud Setup

### Initialize Google Cloud SDK Configuration

1. Install Google Cloud SDK:
   - Follow the instructions on this link: https://cloud.google.com/sdk/docs/install
   - CLI guide: https://cloud.google.com/sdk/gcloud

2. Run `gcloud init` in Terminal and configure default settings:
   - Re-initialize / create new configuration
   - Set configuration name
   - Select / login new google account
   - Select / create new project
   - Select zone [30] asia-southeast1-a
   
3. Create a service account (in Terminal)
    ```
    gcloud iam service-accounts create SERVICE_ACCOUNT_NAME --description="DESCRIPTION" --display-name="DISPLAY_NAME"
    ```

4. Generate a JSON key file for the service account
    ```
    gcloud iam service-accounts keys create /c/set/your/path/KEY_FILE.json --iam-account=SERVICE_ACCOUNT_EMAIL
    ```

5. Update .bash_rc or .bash_profile:
    ```
    export GOOGLE_APPLICATION_CREDENTIALS=/c/Users/thyself/.ssh/service-account-key-file.json
    ```

6. Initialize
    ```
    gcloud init
    gcloud auth application-default login
    gcloud compute ssh instancename --project=projectname --zone=us-central1-a
    ```
