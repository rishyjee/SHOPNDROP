# shopNdrop
The customer need not have to remember all the ingredients required or prick their heads to know what should be next item &amp; will get alert if they are purchasing the item which is already there at home. Use of IoT and Machine learning algorithms to increase the product sells at higher rates. To automate the product purchase by sending the data directly to the particular Super Market.
#shopNdrop
shopNdrop is the demonstration application where it combines Cloud IoT Core and Cloud Machine Learning Engine.

#Requirements 
Google Cloud Platform billing enabled project --
Enable the following APIs
Google Cloud Storage JSON API
Cloud IoT API
BigQuery API
Cloud Machine Learning Engine
Kubernetes Engine API
Raspberry Pi, Camera module and touch display
See Setup Raspberry Pi for more details
#Setup 
Name device ID for a new device and register it to Cloud IoT Core registory
Assemble Raspberry Pi device (see Setup Raspberry Pi for more details)
Built and push Docker container ($ cd gke; docker build -t gcr.io/${PROJECT_ID}/iost-worker .; docker push gcr.io/${PROJECT_ID}/iost-worker)
Create GKE cluster
Deploy workload
Deploy dashboard App Engine application ($ cd dashboard; goapp deploy -application ${PROJECT_ID} -version 1 app.yaml)
