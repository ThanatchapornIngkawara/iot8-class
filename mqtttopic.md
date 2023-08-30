## How do you design MQTT topics and payloads for smart washing machine

1. สถานะเครื่องซักผ้า
    - topic:v1cdti/app/get/6310301007/model-01/sn-001/
    - payload
        - {"STATUS": "POWER ON|START|STOP|FINISHED|POWERED OFF"}
1. เซนเซอร์ภายในเครื่องซักผ้า
    - topic:v1cdti/app/get/6310301007/model-01/sn-001
    - payload
        - {"Temperature": "25.2"}
        - {"Humidity": "50"}
        - {"Time": "60"}
        - {"Airflow": "82"}
        - {"Cool-Down": "5"}
        - {"Pressure": "20"}
        - {"Imbalance": "11"}
        - {"Detergent": "50"}
        - {"noise_anomaly": "40"}
        - {"Rotating": "1000"}
        - {"Water-lavel": "10"}
        - {load": "6"}

 1. เซนเซอร์ภายนอกเครื่องซักผ้า
    - topic:v1cdti/app/get/6310301007/model-01/sn-001
    - payload
        - {"Lid sensor": "off"}
        - {"Child_Lock": "off"}
        - {"Vibration": "20"}
        - {"Current": "110"}
        


