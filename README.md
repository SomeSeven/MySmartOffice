# My Smart Office

MySmartOffice is a IoT platform to monitor the workplace occupancy in real time.  

## Source code

The source code of the project is organized as shown in the tree below:

```
MySmartOffice
│   README.md   
│
└───devices
│   │   
│   └───counter1
│   │   │───device_registration.py
│   │   │───MQTT_Client.py
│   │   │───MyMQTT.py
│   │   │───sniffer.py
│   │   └────utilities.py
│   └───counterN
│   │   ...
│   │
│   └───device_simulation
│  
└───microservices
│   │
│   └───service_catalog
│   │   │───Dockerfile
│   │   │───requirements.txt
│   │   └───service_catalog.py
│   │  
│   └───service_classifier
│   │   └───model_training
│   │   │───classifier.py
│   │   │───Dockerfile
│   │   │───MQTT_Client.py
│   │   │───MyMQTT.py
│   │   │───nn_model
│   │   └───requirements.txt
│   │   
│   └───service_position
│       │───Dockerfile
│       │───requirements.txt
│       └───service_position.py
│   
└───dashboard
    │───index.html
    │───LICENSE
    │───css
    │───img
    │───js
    │───scss
    └───vendor
```

## Running the demo

The dashboard is running online at the following URL:

<http://www.iotgroup28.it>

The code in the folder devices is running on a RaspberryPi, altough its behaviour could be simulated using scripts inside device_simulation folder.

Regarding the classifier, the dataset, the training code and the model used have been included inside the folder service_classifier.

All the microservices developed have been dockerized, so that they could run on every machine with Docker.

## Credits
Serena Celano

Domenico Galdiero

Tommaso Gonella

## License
[MIT](https://choosealicense.com/licenses/mit/)#   M y S m a r t O f f i c e  
 