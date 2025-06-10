# HTTPS Content-Based Load Balancer with Terraform || [GSP206](https://www.cloudskillsboost.google/games/5416/labs/35111) ||

## # Like, comment, share & Don't forget to subscribe [Qwiklab_Explorers](https://youtube.com/@qwiklabexplorers?si=QGN7mY2Sn9iobmuz) 👍😄🤝

---
## ⚠️ **Disclaimer:**
#### This script and guide are provided for educational purposes to help you understand the lab process. Please ensure you understand the steps before using any scripts. Before using the script, I encourage you to open and review it to understand each step.The goal is to help you learn how to complete the labs effectively while following Qwiklabs' terms of service and YouTube's community guidelines.
---

 - ### Copy & Run the Commands in Cloud Shell Terminal :

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

---

## Congratulations ..!!🎉  You completed the lab shortly..😃💯

## *Well done..!* 👏

## Thank you for visiting.... :) 🗯️

## [Qwiklab_Explorers](https://youtube.com/@qwiklabexplorers?si=QGN7mY2Sn9iobmuz)

## Join to our community [Digital Dominators](https://linktr.ee/digital_dominators)
