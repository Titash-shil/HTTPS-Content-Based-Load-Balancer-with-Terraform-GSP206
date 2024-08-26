# HTTPS Content-Based Load Balancer with Terraform || [GSP206](https://www.cloudskillsboost.google/games/5416/labs/35111) ||

# # Like, comment, share & Don't forget to subscribe [Qwiklab_Explorers_ts](https://youtube.com/@titashshil?si=RgamNu1dc9jVIbJN) 👍😄🤝

### Run the following Commands in CloudShell

```
gcloud auth list

export PROJECT_ID=$(gcloud config get-value project)

export PROJECT_ID=$DEVSHELL_PROJECT_ID

git clone https://github.com/GoogleCloudPlatform/terraform-google-lb-http.git

cd ~/terraform-google-lb-http/examples/multi-backend-multi-mig-bucket-https-lb

rm -rf main.tf

wget https://raw.githubusercontent.com/Titash-shil/HTTPS-Content-Based-Load-Balancer-with-Terraform-GSP206/main/GSP206%20-main.tf

terraform init

terraform plan -var project=$DEVSHELL_PROJECT_ID
ls
terraform apply -var project=$DEVSHELL_PROJECT_ID -auto-approve


sleep 10

EXTERNAL_IP=$(terraform output | grep load-balancer-ip | cut -d = -f2 | xargs echo -n)
echo https://${EXTERNAL_IP}

```

* ## Go to `BigQuery` from [here](https://console.cloud.google.com/bigquery?)

# Congratulations ..!!🎉  You completed the lab shortly..😃💯

# *Well done..!* 👏

# Thank you for visiting.... :) 🗯️

# [Qwiklab_Explorers_ts](https://youtube.com/@titashshil?si=RgamNu1dc9jVIbJN)
