# Aegis-Mint-Auth8-Deployment
# Aegis Mint Authentication Service (CLI Deployment Guide)  This repository contains the official command-line interface (CLI) deployment assets and instructions for running the **Aegis Mint Authentication** service on Google Cloud.
File 1: README.md
# Aegis Mint Authentication Service (CLI Deployment Guide)
This repository contains the official command-line interface (CLI) deployment assets and instructions for running the **Aegis Mint Authentication** service on Google Cloud.
## Prerequisites
Before deploying, ensure you have the following ready:
1. A Google Cloud Platform (GCP) project with billing enabled.
2. The Google Cloud CLI (`gcloud`) installed and authenticated. 
   - [Install gcloud CLI](https://cloud.google.com/sdk/docs/install)
3. Enabled APIs in your target GCP project:
   - Cloud Run API (`run.googleapis.com`)
---
## Quickstart Deployment via CLI
You can easily deploy the Aegis Mint Authentication service to Google Cloud Run using the `gcloud` CLI. 
### Step 1: Clone this Repository
```bash
git clone https://github.com/Solomonltd/Aegis-Mint-Auth8-Deployment.git
cd Aegis-Mint-Auth8-Deployment
# Aegis Mint Authentication Service (CLI Deployment Guide)

This repository contains the official command-line interface (CLI) deployment assets and instructions for running the **Aegis Mint Authentication** service on Google Cloud.

## Prerequisites

Before deploying, ensure you have the following ready:
1. A Google Cloud Platform (GCP) project with billing enabled.
2. The Google Cloud CLI (`gcloud`) installed and authenticated. 
   - [Install gcloud CLI](https://cloud.google.com/sdk/docs/insta
Generated code may be subject to license restrictions not shown here. Use code with care. Learn more 

Step 2: Configure your GCP Environment
Set your active project and choose your preferred region (e.g., us-central1 or europe-west1):

gcloud config set project <YOUR_PROJECT_ID>
export REGION="us-central1"
gcloud config set project <YOUR_PROJECT_ID>
export REGION="us-central1"
Generated code may be subject to license restrictions not shown here. Use code with care. Learn more 

Step 3: Deploy to Cloud Run
Run the following command to pull the certified deployer image and deploy it directly to Cloud Run:

gcloud run deploy aegis-mint-auth-service \
    --image=us-docker.pkg.dev/solomobn-nexus/aegis-mint-docker/deployer:1.0.0 \
    --region=$REGION \
    --port=3000 \
    --allow-unauthenticated
gcloud run deploy aegis-mint-auth-service \
    --image=us-docker.pkg.dev/solomobn-nexus/aegis-mint-docker/deployer:1.0.0 \
    --region=$REGION \
    --port=3000 \
    --allow-unauthenticated
Generated code may be subject to license restrictions not shown here. Use code with care. Learn more 

Configuration Settings
You can customize the deployment by passing additional flags during the gcloud run deploy command:

Parameter   Flag  Description Default
Port  --port   The port your application container listens on  3000
Min Instances  --min-instances   Minimum number of warm container instances   0
Max Instances  --max-instances   Maximum number of containers during traffic spikes 100
Support & Documentation
For full documentation and advanced configuration guides, please visit our official support portal at https://solomonltd.com/support .

---
### What to do next:
1.  **Create your new public GitHub repository** (e.g., `Aegis-Mint-Auth8-Deployment`).
2.  Add a **`README.md`** file, paste the template above, and commit it.
3.  **Copy the public repository URLs:**
    *   **Public git repo URL:** `https://github.com/Solomonltd/Aegis-Mint-Auth8-Deployment`
    *   **Deploy documentation URL:** `https://github.com/Solomonltd/Aegis-Mint-Auth8-Deployment/blob/main/README.md`
4.  Paste these two links into your Google Cloud Marketplace form and click **Save**!
Once you save, is there any other subtask on the checklist or other forms you need help filling out?
