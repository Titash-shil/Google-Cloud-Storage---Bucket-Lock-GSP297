# Google Cloud Storage - Bucket Lock || [GSP297](https://www.cloudskillsboost.google/focuses/3483?parent=catalog) ||

# # Like, comment, share & Don't forget to subscribe [Qwiklab_Explorers_ts](https://youtube.com/@titashshil?si=RgamNu1dc9jVIbJN) 👍😄🤝

### Run the following Commands in CloudShell

```
export BUCKET=$(gcloud config get-value project)

gsutil mb "gs://$BUCKET"

sleep 5

gsutil retention set 10s "gs://$BUCKET"

gsutil retention get "gs://$BUCKET"

gsutil cp gs://spls/gsp297/dummy_transactions "gs://$BUCKET/"

gsutil ls -L "gs://$BUCKET/dummy_transactions"

sleep 5

gsutil retention lock "gs://$BUCKET/"

gsutil retention temp set "gs://$BUCKET/dummy_transactions"

gsutil rm "gs://$BUCKET/dummy_transactions"

gsutil retention temp release "gs://$BUCKET/dummy_transactions"

gsutil retention event-default set "gs://$BUCKET/"

gsutil cp gs://spls/gsp297/dummy_loan "gs://$BUCKET/"

gsutil ls -L "gs://$BUCKET/dummy_loan"

gsutil retention event release "gs://$BUCKET/dummy_loan"

gsutil ls -L "gs://$BUCKET/dummy_loan"
```

# Congratulations ..!!🎉  You completed the lab shortly..😃💯

# *Well done..!* 👏

# Thank you for visiting.... :) 🗯️

# [Qwiklab_Explorers_ts](https://youtube.com/@titashshil?si=RgamNu1dc9jVIbJN)
