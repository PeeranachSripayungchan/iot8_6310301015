## How do you design MQTT topics and payloads for smart washing machine

1. สถานะเครื่องซักผ้า
    - topic:v1cdti/app/get/6310301015/model-01/sn-001/
    - payload
        - {"STATUS": "POWER ON|START|STOP|FINISHED|POWERED OFF"}
1. เซนเซอร์ภายในเครื่องซักผ้า
    - topic:v1cdti/app/get/6310301015/model-01/sn-001
    - payload
        - {"temperature": "25.2"}
        - {"pressure": "50"}
        - {"water_volume": "2}
        - {"weight": "1.5"}
        - {"lid": "open"}
        - {"air_pressure": "20"}
        - {"noise": "80"}
        - {"foam": "40"}

## temperature (Celcius)
## pressure (Pascal)
## water_volume (liter)
## weight (kilogram)
## lid (open/close)
## air_pressure (Pascal)
## noise (decibel)
## foam (percent)

 1. เซนเซอร์ภายนอกเครื่องซักผ้า
    - topic:v1cdti/app/get/6310301015/model-01/sn-001
    - payload
        - {"noise": "80"}
        - {"outer_air_pressure": "20"}
        - {"relative_humidity": "60"}

## noise (decibel)
## outer_air_pressure (Pascal)
## relative_humidity (percent)


