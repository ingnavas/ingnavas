 Jaime Eduardo Navarrete – Curriculum Vitae

## Projects

## 2025  
### 🖼️ Sistema de Monitoramento de Variábles Remotas

**Linguagem:**  
- Python, usando [![Taipy](https://img.shields.io/badge/Taipy-docs-blue?logo=python&logoColor=white)](https://taipy.io/) para server local  

**Hardware:**  
- [![TRB145](https://img.shields.io/badge/Teltonika-TRB145-green?logo=raspberrypi&logoColor=white)](https://teltonika-networks.com/products/gateways/trb145)  
- [![Polilyte](https://img.shields.io/badge/Hamilton-Polilyte%20Plus%20PHI%20Arc%20120-orange?logo=labview&logoColor=white)](https://www.hamiltoncompany.com/product-specs/242428-4313)

<details>
  <summary><b>📜 Ver ejemplo del código en Python </b>></summary>
 
```python
class ToAcquisition:
    """
    Class that represents the variables to be passed initially to the acquisition thread.
    Attributes:
        broker_ip           (str - XXX.XXX.XXX.XX)  =   IP address in VPN-RMS
        port                (int)                   =   port MQTT
        topic_request       (str)                   =   topic name in TRB145
        topic_response      (str)                   =   topic name in TRB145
        serial_device_id    (str)                   =   serial name tag in TRB145
        server_id           (int)                   =   server id Hamilton sensor
        modbus_function     (int)                   =   modbus function
        register_VP         (int)                   =   process variable register
        reg_num             (int)                   =   register numbers process variable for register

    Methods:
    - __init__: Initialize attributes with values ​​provided or by default.
    """
    def __init__(self, broker_ip=None,  port=None, topic_request = None,
    topic_response=None, serial_device_id=None, server_id=None,  
    modbus_function=None, first_register = None, reg_num=None):

        self.broker_ip          =   broker_ip
        self.port               =   port
        self.topic_request      =   topic_request
        self.topic_response     =   topic_response
        self.serial_device_id   =   serial_device_id
        self.server_id          =   server_id
        self.modbus_function    =   modbus_function
        self.first_register     =   first_register
        self.reg_num            =   reg_num


# Defines the object used to pass initial information to the thread

to_acquisition = ToAcquisition()
to_acquisition.broker_ip          =   "192.168.255.6"         # IP in VPN RMS
to_acquisition.port               =   1883                    # Default MQTT port
to_acquisition.topic_request      =   "request/modbus"        # topic name in TRB145
to_acquisition.topic_response     =   "response/modbus"       # topic name in TRB145
to_acquisition.serial_device_id   =   "redeEL" 
to_acquisition.server_id          =   1
to_acquisition.modbus_function    =   3
to_acquisition.first_register     =   2410
to_acquisition.reg_num            =   10

...{more code}


def on_init(state):
    invoke_long_callback(state=state,
                                user_function=acquisition, user_function_args=[state.gui, get_state_id(state), state.to_acquisition],
                                user_status_function=status_fct, user_status_function_args=[])
```

</details> 


sadasda
