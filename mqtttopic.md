## How do you design MQTT topics and payloads for smart washing machine

1. สถานะเครื่องซักผ้า
    - topic:v1cdti/app/get/1212312121/model-01/sn-001/
    - payload
        - {"STATUS": "POWER ON|START|STOP|FINISHED|POWERED OFF"}
1. เซนเซอร์ภายในเครื่องซักผ้า
    - topic:v1cdti/app/get/1212312121/model-01/sn-001
    - payload
        - {"temperature": "25.2"}
        - {"pressure": "20"}
        - {"water level": "2"}
        - {"3-D Positin sensor": "2,2,0"}
        - {"humanity": "10"}
        - {"ordor": "normal"}
        - {"water": "0"}
        - {"smoke": "Y"}
        - {"quantity": "6"}
        

 1. เซนเซอร์ภายนอกเครื่องซักผ้า
    - topic:v1cdti/app/get/1212312121/model-01/sn-001
    - payload
        - {"Radar": "Y"}
        - {"humanity": "0"}
        - {"temperature": "30"}
        - {"door position": "close"}
        - {"button": "Y"}
        - {"touch": "Y"}
        - {"condition monitoring": "3"}



