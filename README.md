# shopNdrop
The customer need not have to remember all the ingredients required or prick their heads to know what should be next item &amp; will get alert if they are purchasing the item which is already there at home. Use of IoT and Machine learning algorithms to increase the product sells at higher rates. To automate the product purchase by sending the data directly to the particular Super Market.
#shopNdrop
shopNdrop is the demonstration application where it combines Cloud IoT Core and Cloud Machine Learning Engine.

# Requirements 
Google Cloud Platform billing enabled project </br>
Enable the following APIs</br>
Google Cloud Storage JSON API</br>
Cloud IoT API</br>
BigQuery API</br>
Cloud Machine Learning Engine</br>
Kubernetes Engine API</br>
Raspberry Pi, Camera module and touch display</br>
See Setup Raspberry Pi for more details</br>
# Setup 
Name device ID for a new device and register it to Cloud IoT Core registory</br>
Assemble Raspberry Pi device (see Setup Raspberry Pi for more details)</br>
Built and push Docker container ($ cd gke; docker build -t gcr.io/${PROJECT_ID}/iost-worker .; docker push gcr.io/${PROJECT_ID}/iost-worker)</br>
Create GKE cluster</br>
Deploy workload</br>
Deploy dashboard App Engine application ($ cd dashboard; goapp deploy -application ${PROJECT_ID} -version 1 app.yaml)
