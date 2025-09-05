 Jaime Eduardo Navarrete – Curriculum Vitae

## Proyectos

<!-- PRIMER PROYECTO -->

## 2025  
### Sistema de Monitoramento de Variábles Remotas

En esta applicación de realiza una comunicación con un gateway GSM/Modbus para colectar datos de un sensor remoto y se realiza una visualización en un server local

**Caracteristicas:**  
- Lenguaje python
- Frontend en [![Taipy](https://img.shields.io/badge/Taipy-gui-blue?logo=python&logoColor=white)](https://taipy.io/) usando server local
- Comunicación modbus RTU e MQQT

**Hardware:**  

- [![TRB145](https://img.shields.io/badge/Teltonika-TRB145-green?logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjIwIiBoZWlnaHQ9IjIyMCIgdmlld0JveD0iMCAwIDIyMCAyMjAiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CiAgPHBvbHlnb24gcG9pbnRzPSI0MCwxMTAgMTEwLDQwIDE1MCw4MCA4MCwxNTAiIGZpbGw9Im5vbmUiIHN0cm9rZT0iYmxhY2siIHN0cm9rZS13aWR0aD0iMTAiLz4KICA8cG9seWdvbiBwb2ludHM9IjgwLDExMCAxNTAsNDAgMTkwLDgwIDEyMCwxNTAiIGZpbGw9Im5vbmUiIHN0cm9rZT0iYmxhY2siIHN0cm9rZS13aWR0aD0iMTAiLz4KICA8cG9seWdvbiBwb2ludHM9IjEyMCwxMTAgMTkwLDQwIDIyMCw3MCAxNTAsMTUwIiBmaWxsPSJub25lIiBzdHJva2U9ImJsYWNrIiBzdHJva2Utd2lkdGg9IjEwIi8+Cjwvc3ZnPg==)](https://teltonika-networks.com/products/gateways/trb145)

- [![Polilyte](https://img.shields.io/badge/Hamilton-Polilyte%20Plus%20PHI%20Arc%20120-orange?logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTIwIiBoZWlnaHQ9IjEyMCIgdmlld0JveD0iMCAwIDEyMCAxMjAiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CiAgPGNpcmNsZSBjeD0iNjAiIGN5PSI2MCIgcj0iNTgiIGZpbGw9IiMyMTJGNEEiIC8+CiAgPHRleHQgeD0iNTAlIiB5PSI2MiUiIGRvbWluYW50LWJhc2VsaW5lPSJtaWRkbGUiIHRleHQtYW5jaG9yPSJtaWRkbGUiCiAgICAgICAgZm9udC1mYW1pbHk9IkJydXNoIFNjcmlwdCBNVCwgQnJ1c2hTY3JpcHRNVCwgY3Vyc2l2ZSIKICAgICAgICBmb250LXNpemU9IjgwIiBmaWxsPSIjZmZmIj4KICAgIEgKICA8L3RleHQ+Cjwvc3ZnPg==)](https://www.hamiltoncompany.com/product-specs/242428-4313)


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


<details>
  <summary><b>📜 Aplicación </b>></summary>

![Monitoreo remoto](https://drive.google.com/uc?export=view&id=1L07g0xDrygkLB1vOwiCdOPpOJMcvkvYx)

</details>

---
<!-- SEGUNDO PROYECTO -->

### Clasificador de tamaño de partículas en cristalización

En esta applicación de realiza una clasificación del tamaño de particulas en un proceso de cristalización

**Caracteristicas:**  
- Lenguaje python
- Frontend en [![Taipy](https://img.shields.io/badge/Taipy-gui-blue?logo=python&logoColor=white)](https://taipy.io/) usando server local
- OpenCV
- Banco de datos SQLite

**Hardware:**  

No aplica, usa imagenes provenientes de cualquier microscopio, teniendo una referencia de distancia de medida

<details>
  <summary><b>📜 Ver ejemplo del código en Python </b>></summary>
 
```python
#@BRIEF:                    Realiza la calibración manual
#@PARAM state:              Variables de estado de la instancia
def manual_calibration(state):
    drawing = False  # verdadero si el mouse es presionado
    ix, iy = -1, -1  # coordenadas iniciales
    img_gray= cv2.imread(state.content_load_calibration, cv2.IMREAD_GRAYSCALE)
    img = cv2.cvtColor(img_gray, cv2.COLOR_GRAY2BGR)
    img_copy = img.copy()

    # funcion de llamada el mouse
    def draw_line(event, x, y, flags, param):
        nonlocal ix, iy, drawing, img_copy

        if event == cv2.EVENT_LBUTTONDOWN:
            drawing = True
            ix, iy = x, y

        elif event == cv2.EVENT_MOUSEMOVE:
            if drawing:
                img_copy = img.copy()
                cv2.line(img_copy, (ix, iy), (x, y), (0, 255, 0), 2)
                cv2.putText(img_copy, f"Inicio: ({ix},{iy})", (10, 100),
                            cv2.FONT_HERSHEY_SIMPLEX, 3, (255, 255, 255), 5)
                cv2.putText(img_copy, f"Fin: ({x},{y})", (10, 200),
                            cv2.FONT_HERSHEY_SIMPLEX, 3, (255, 255, 255), 5)

        elif event == cv2.EVENT_LBUTTONUP:
            drawing = False
            cv2.line(img_copy, (ix, iy), (x, y), (0, 255, 0), 8)
            state.point_x1=ix
            state.point_y1=iy
            state.point_x2=x
            state.point_y2=y

            print(f"Line drawn from ({ix}, {iy}) to ({x}, {y})")
            cv2.putText(img_copy, f"Inicio: ({ix},{iy})", (10, 100),
                        cv2.FONT_HERSHEY_SIMPLEX, 3, (255, 255, 255), 5)
            cv2.putText(img_copy, f"Fin: ({x},{y})", (10, 200),
                        cv2.FONT_HERSHEY_SIMPLEX, 3, (255, 255, 255), 5)

    # Set up window
    cv2.namedWindow("Draw Line", cv2.WINDOW_NORMAL)
    cv2.setMouseCallback("Draw Line", draw_line)
    cv2.setWindowProperty("Draw Line", cv2.WND_PROP_TOPMOST, 1)  

    while True:
        cv2.imshow("Draw Line", img_copy)

        if cv2.waitKey(1) & 0xFF == 13: # ENTER key (13)
            break

    cv2.destroyAllWindows()
    
    cv2.line(img, (state.point_x1, state.point_y1), (state.point_x2, state.point_y2), (0, 255, 0), 8)
    cv2.imwrite("cal_man.png", img)
    state.um_per_pixel = int(state.micrometer_spacing)*int(state.lines_number)/ int(abs(state.point_x2-state.point_x1))
    state.um_per_pixel=state.um_per_pixel
    state.content_show_calibration="cal_man.png"
    state.content_show_calibration=state.content_show_calibration
    notify(state, "warning", f"🪜 Verifique el número de intervalos usados")
    state.cal_from='Manual'
```

</details> 


<details>
  <summary><b>📜 Aplicación </b>></summary>

![Cristalización](https://drive.google.com/uc?export=view&id=1FBPtxAnipIjrpIgO9ms8j3TBNU5uLvnN)

</details>

---

<!-- TERCER PROYECTO -->

### Software para ensayo DSL (Dynamic Scale Loop)

En esta applicación comanda el equipo para análisis DSL, modelo MTDE de la empresa Biofoco Equipamentos para Laboratórios de Brasil

**Caracteristicas:**  
- Lenguaje python
- Frontend en [![Taipy](https://img.shields.io/badge/Taipy-gui-blue?logo=python&logoColor=white)](https://taipy.io/) usando server local
- Comunicación modbus RTU, y protocolo propio de Jasco en RS232
- Algoritmo de control de temperatura en cascada
- Procesamiento paralelo en  [![threads](https://img.shields.io/badge/Threads-parelelismo-gui-gray?)](https://www.linkedin.com/pulse/taipy-integration-data-acquisition-systems-navarrete-rodriguez-d7igc/?trackingId=WMqY4PWJRASx%2FvyMkzbxWg%3D%3D) 




**Hardware:**  

- [![Bombas HPLC](https://img.shields.io/badge/Jasco-Bombas-yellow?)](https://jascoinc.com/products/chromatography/hplc/modules/hplc-pumps/)

- [![Fieldlogger](https://img.shields.io/badge/Novus-Fieldlogger-green?)](https://www.novus.com.br/pt/produto/data-loggers/fieldlogger)

- [![Controlador](https://img.shields.io/badge/Novus-Controlador%20N120S-orange?)](https://www.novus.com.br/site/default.asp?TroncoID=508083&secaoID=547383&SubSecaoID=727292&Template=../catalogos/layout_produto.asp&ProdutoID=293738)

- [![Transmisor](https://img.shields.io/badge/Yokogawa-Presi%C3%B3n%20diferencial-orange?)](https://www.yokogawa.com/br/solutions/products-and-services/measurement/field-instruments-products/pressure-transmitters/differential-pressure/eja110e/)

- [![Transmisor](https://img.shields.io/badge/Velki-Presi%C3%B3n%20manom%C3%A9trica-blue?)](https://velki.com.br/pt/produto/medidores-de-pressao/transmissores-de-pressao/transmissor-de-pressao-mini-ip65-ceramico---vkp-091)



<details>
  <summary><b>📜 Ver ejemplo del código en Python </b>></summary>
 
```python

class PIDController:
    def __init__(self, Kp, Ki, Kd, T,Kaw, output_limits=(-float('inf'), float('inf'))):
        """
        PID Controller with anti-windup and bumpless transfer.

        Parameters:
        - Kp (float): Proportional gain
        - Ki (float): Integral gain
        - Kd (float): Derivative gain
        - T (float): Sampling time (seconds)
        - output_limits (tuple): Min and max output limits (anti-windup)
        """
        self.Kp = Kp
        self.Ki = Ki
        self.Kd = Kd
        self.T = T
        self.output_limits = output_limits
        
        # Internal states
        self.integral = 0.0
        self.prev_error = 0.0
        self.prev_output = 0.0
        self.prev_derivative = 0.0
        self.setpoint = 0.0  # Desired value
        
        # Anti-windup
        self.I_term = 0.0  # Integral term for bumpless transfer
        self.Kaw = Kaw  # Anti-windup coefficient

    def update(self, measurement):
        """
        Computes the PID control action.
        
        Parameters:
        - measurement (float): Process variable (PV)

        Returns:
        - control_output (float): PID output
        """
        error = self.setpoint - measurement
        # Proportional term
        P_term = self.Kp * error

        # Integral term with anti-windup
        self.I_term += self.Ki * error * self.T
        self.I_term -= self.Kaw * (self.prev_output - self.clamp(self.prev_output))  # Anti-windup correction
        
        # Derivative term (using backward difference)
        derivative = (error - self.prev_error) / self.T
        D_term = self.Kd * derivative
        
        # Compute total output
        output = P_term + self.I_term + D_term

        self.prev_output = output
        # Apply output limits (clamping)
        output = self.clamp(output)

        # Store values for next iteration
        self.prev_error = error
        self.prev_derivative = derivative

        return output

    def clamp(self, value):
        """
        Limits the output to avoid integral windup.
        """

        min_output, max_output = self.output_limits
        return max(min(value, max_output), min_output)

    def set_setpoint(self, new_setpoint):
        """
        Updates the setpoint with bumpless transfer.
        
        Parameters:
        - new_setpoint (float): Desired setpoint
        """
        delta_setpoint = new_setpoint - self.setpoint
        self.setpoint = new_setpoint
        self.I_term += delta_setpoint * self.Ki * self.T  # Bumpless transfer for integral action

pid = PIDController(kc, ti, td, tempo_amostra_cascata,reset_aw, output_limits=(sat_min, sat_max))


```

</details> 


<details>
  <summary><b>📜 Aplicación </b>></summary>

![Cristalización](https://drive.google.com/uc?export=view&id=1jBoOb9EYk22-cXdPvHVymaITFLeRyFqR)


</details>

