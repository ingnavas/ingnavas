
## Hello
## 👋 I’m Jaime Eduardo Navarrete   [![español](https://img.shields.io/badge/lang-es-yellow)](#hola) [![proyectos](https://img.shields.io/badge/projects-all-blue)](#últimos-proyectos-o-proyectos-importantes--)

### 🔧 About Me 

I design solutions for data acquisition from physical systems through hardware and software integration.

Rather than labeling myself strictly as a "programmer," I see myself as a problem solver for data acquisition — someone who learns and applies the necessary knowledge to tackle real-world challenges.

Over the years, I have worked extensively with:

* Programming tools: Python (since 2021), Object Pascal – Delphi (since 2001), LabVIEW (since 1998), Matlab (since 1997)

* HMI development for industrial and laboratory applications in DOPSoft IDE (Delta Electronics) (since 2013)

* Integration of hardware and software for reliable measurement systems (since 1999)

### 📊 Data Acquisition Expertise 

I have hands-on experience designing and implementing data acquisition systems for a wide range of physical variables, including all common measurements in industrial environments such as Pressure, Temperature, pH, RPM, Dissolved Oxygen, and Turbidity, among others.

Additionally, I have some hands-on experience in image analysis for laboratory applications.

This expertise allows me to bridge the gap between sensors, hardware, and intelligent software, ensuring accurate and reliable information flow from the physical world to decision-making systems.

### 🎓 Academic Background 

I am Chemical Engineering, but I hold a PhD in Electrical Engineering in the area of Control Systems, including:

* Classical Control (PID, cascade, etc.).

* Advanced Control (Predictive and Adaptive Control).

* System Identification for dynamic modeling of physical and chemical processes.

And for two separate periods (2011 to 2012 and 2016 to 2018), I was a professor at São Paulo State University (UNESP), Brazil, teaching courses in industrial process control

This strong academic background complements my engineering experience, enabling me to design robust and scalable solutions that meet industrial demands.

### ⚙️From Lab to Industry 

By combining my Data Acquisition Expertise with my Academic Background in control and system identification, I deliver solutions that:

* Enhance process monitoring and automation.

* Enable predictive and adaptive control strategies.

* Provide scalable architectures for industrial and laboratory environments.

* Transform raw sensor data into actionable insights for decision-making.

## 🧩 In short 
**I bring the rigor of research and the practicality of engineering to create innovative solutions for industrial challenges — measuring the real world to enable better decisions about it.**


<hr style="height:3px; background-color:#000; border:none;" />


## Hola

## 👋 Soy Jaime Eduardo Navarrete  [![english](https://img.shields.io/badge/lang-en-yellow)](#hello) [![proyectos](https://img.shields.io/badge/proyectos-todos-blue)](#últimos-proyectos-o-proyectos-importantes--)

### 🔧 Sobre mí 

Diseño soluciones para la adquisición de datos de sistemas físicos mediante la integración de hardware y software.

Más que definirme estrictamente como “programador”, me considero un solucionador de problemas de adquisición de datos — alguien que aprende y aplica el conocimiento necesario para enfrentar desafíos reales.

A lo largo de los años, he trabajado extensamente con:

* Lenguajes y herramientas de programación: Python (desde 2021), Object Pascal – Delphi (desde 2001), LabVIEW (desde 1998), Matlab (desde 1997)

* Desarrollo de interfaces HMI para aplicaciones industriales y de laboratorio en DOPSoft IDE (Delta Electronics) (desde 2013)

* Arduino (desde 2010) y ESP32 (desde 2018)

* Integración de hardware y software para sistemas de medición confiables (desde 1999)

### 📊 Experiencia en Adquisición de Datos 

Tengo experiencia práctica en el diseño e implementación de sistemas de adquisición de datos para una amplia gama de variables físicas, incluyendo todas las más comunes en entornos industriales como Presión, Temperatura, pH, RPM, Oxígeno Disuelto y Turbidez, entre otras.

Además, cuento con algo de experiencia en análisis de imágenes aplicado a entornos de laboratorio.

Esto me permite cerrar la brecha entre sensores, hardware y software inteligente, garantizando un flujo de información preciso y confiable desde el mundo físico hasta los sistemas de toma de decisiones.

### 🎓Formación Académica 

Soy Ingeniero Químico mas concluí mi doctorado en Ingeniería Eléctrica (2010), en el área del conocimiento que abarca:

* Control Clásico (PID, en cascada, etc.).

* Control Avanzado (Predictivo y Adaptativo).

* Identificación de Sistemas para el modelado dinámico de procesos físicos y químicos.

Y por un dos periódos separados (2011 a 2012 y 2016 a 2018) fui profesor en universidad del estado de São Paulo (UNESP), Brasil en las disciplinas de control de procesos industriales.

Esta sólida formación académica complementa mi experiencia en ingeniería, lo que me permite diseñar soluciones robustas y escalables que responden a las demandas industriales.

### ⚙️Del Laboratorio a la Industria 

Al combinar mi experiencia en adquisición de datos con mi formación académica en control e identificación de sistemas, entrego soluciones que:

* Mejoran el monitoreo y la automatización de procesos.

* Permiten estrategias de control predictivo y adaptativo.

* Ofrecen arquitecturas escalables para entornos industriales y de laboratorio.

* Transforman los datos de sensores en información para la toma de decisiones.

### 🧩 En resumen 

Aporto el rigor de la investigación y la practicidad de la ingeniería para crear soluciones innovadoras a los desafíos industriales — midiendo el mundo real para poder tomar mejores decisiones sobre él.

<hr style="height:5px; background-color:blue; border:none; width:50%;" />


## Últimos proyectos o proyectos importantes [![english](https://img.shields.io/badge/lang-en-yellow)](#hello) [![español](https://img.shields.io/badge/lang-es-yellow)](#hola)

<!-- PRIMER PROYECTO -->

## 2025  
### Sistema de Monitoramento de Variábles Remotas

Esta aplicación  comunica con un gateway GSM/Modbus para colectar datos de un sensor remoto y realiza una visualización de datos.

**Caracteristicas:**  
- Lenguaje: [![Python](https://img.shields.io/badge/Python-daq-blue?logo=python&logoColor=white)](https://www.python.org/).
- Frontend: [![Taipy](https://img.shields.io/badge/Taipy-gui-blue?logo=taipy&logoColor=white)](https://taipy.io/) usando server local.
- Comunicación:  MQQT/Modbus RTU. 

**Hardware:**  

- [![TRB145](https://img.shields.io/badge/Teltonika-TRB145-green)](https://teltonika-networks.com/products/gateways/trb145).

- [![Polilyte](https://img.shields.io/badge/Hamilton-Polilyte%20Plus%20PHI%20Arc%20120-orange)](https://www.hamiltoncompany.com/product-specs/242428-4313).


<details>
 
  <summary><b>🔽 Ver código / 🔼 Ocultar código</b></summary>
 
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

Esta aplicación realiza la clasificación del tamaño de particulas a partir de imagenes de un proceso de cristalización durante un determinado intervalo de tiempo. Ejecuta en un server local con lectura off-line.

**Caracteristicas:**  
- Lenguaje python.
- Frontend en [![Taipy](https://img.shields.io/badge/Taipy-gui-blue?logo=python&logoColor=white)](https://taipy.io/) usando server local.
- OpenCV.
- Banco de datos SQLite.

**Hardware:**  

No aplica, usa imagenes provenientes de cualquier microscopio, teniendo una referencia de distancia de medida.

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
## 2024

### Software para ensayo DSL (Dynamic Scale Loop)

Esta applicación comanda el equipo para análisis DSL, modelo MTDE de la empresa Biofoco Equipamentos para Laboratórios de Brasil. Ejecuta en un server local con lectura on-line.

**Caracteristicas:**  
- Lenguaje python.
- Frontend en [![Taipy](https://img.shields.io/badge/Taipy-gui-blue?logo=python&logoColor=white)](https://taipy.io/) usando server local.
- Comunicación modbus RTU, y protocolo propio de Jasco en RS232.
- Algoritmo de control de temperatura en cascada.
- Procesamiento paralelo en  [![Threads](https://img.shields.io/badge/Threads-paralelismo-green)](https://www.linkedin.com/pulse/taipy-integration-data-acquisition-systems-navarrete-rodriguez-d7igc/?trackingId=WMqY4PWJRASx%2FvyMkzbxWg%3D%3D).


**Hardware:**  

- [![Bombas HPLC](https://img.shields.io/badge/Jasco-Bombas-yellow?)](https://jascoinc.com/products/chromatography/hplc/modules/hplc-pumps/).

- [![Fieldlogger](https://img.shields.io/badge/Novus-Fieldlogger-green?)](https://www.novus.com.br/pt/produto/data-loggers/fieldlogger).

- [![Controlador](https://img.shields.io/badge/Novus-Controlador%20N120S-orange?)](https://www.novus.com.br/site/default.asp?TroncoID=508083&secaoID=547383&SubSecaoID=727292&Template=../catalogos/layout_produto.asp&ProdutoID=293738).

- [![Transmisor](https://img.shields.io/badge/Yokogawa-Presi%C3%B3n%20diferencial-orange?)](https://www.yokogawa.com/br/solutions/products-and-services/measurement/field-instruments-products/pressure-transmitters/differential-pressure/eja110e/).

- [![Transmisor](https://img.shields.io/badge/Velki-Presi%C3%B3n%20manom%C3%A9trica-blue?)](https://velki.com.br/pt/produto/medidores-de-pressao/transmissores-de-pressao/transmissor-de-pressao-mini-ip65-ceramico---vkp-091).


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

![DSL/MTED](https://drive.google.com/uc?export=view&id=1jBoOb9EYk22-cXdPvHVymaITFLeRyFqR)


</details>

<!-- CUARTO PROYECTO -->
## 2022/2023

### API Angejiga + API ESP32-Modbus + STlink class 

Dos APIs y una clase dedicada componen este proyecto para la programación de productos baseados en microcontroladores ST y el control de calidad de placas electrónicas en el proceso de ensamblado de estas.

La API Angejiga es solución personalizada para lectura/escrita de entradas analógicas y digitales, usando un hardware personalizado basado en Arduino Mega, denominado por el cliente como Angejiga. Asi, el programador responsable puede concentrarse en la lógica del ensayo de alto nível sin la preocupación de los mapeamentos de lecturas y accionamientos del hardware. 

La API ESP32-Modbus es solución personalizada, usada en la programación de firmware para diferentes tipos de microcontroladores, para proporcionar aislamiento en los sistemas de gravación. Esta permite una comunicación modbus via wi-fi para control de lógica de grabación

La clase STlink permite un control de gravación de los microcontroladores STMicroelectronics a través del uso de lineas de comando ( Command Line Interface)


**Caracteristicas:**  
- API Angejiga en lenguaje python con biblioteca firmata del lado del arduino mega
- API ESP32-Modbus programada en IDE del Arduino
- Frontend del producto de cliente en [![Taipy](https://img.shields.io/badge/Taipy-gui-blue?logo=python&logoColor=white)](https://taipy.io/) usando server local.


**Hardware:**  

- Angejiga  desarrollado por el cliente
- Placa gravadores desarrollada por el cliente

<details>
  <summary><b>📜 Ver ejemplo del código de la API Angejiga en Python </b>></summary>
 
```python
#@BRIEF: CLASSE ATRELADA AO HARDWARE DA JIGA - VER MAPEAMENTO DA JIGA
# @Remarks:  
#       Ao criar o objeto sempre será necessario após inicialização chamar o util.iterator e it.start
#       Deve-se importar o util
#           Jiga=JigaAngejiga()
#           it = util.Iterator(Jiga.DAQ)
#           it.start()
class JigaAngejiga:
    """
    CLASSE PARA USO DE HARDWARE ANGEJIGA 
    
        Através de esta classe é realizada a definição de entradas/saídas analógicas e 
        digitais usadas no shield Angejiga desenvolvido para Jigas de teste
    
    ATRIBUTOS

        NÃO ATRELADOS A HARDWARE

            * posJumpers (0b:int16)

            * DAQ (pyfirmata.ArduinoMega)   : A placa arduino do projeto.

            * vutil (module)                : módulo de tratativa de dados.

            * it (pyfirmata.util.Iterator)  : classe de thread para leituras de dados analógicos e digitais.

        CONETOR CN18
        
            * AC_DOUT0 (int)                        = 25    : saída AC dígital 0  (Fase CN18:8 Neutro CN18:7)
            * I_AC_DOUT0 (pyfirmata.pyfirmata.Pin)  = 11    : corrente na saída AC digital 0  
            * AC_DOUT1 (int)                        = 24    : saída AC dígital 1  (Fase CN18:6 Neutro CN18:5)
            * I_AC_DOUT1 (pyfirmata.pyfirmata.Pin)  = 10    : corrente na saída AC digital 1          
            * AC_DOUT2 (int)                        = 23    : saída AC dígital 2  (Fase CN18:4 Neutro CN18:3)
            * I_AC_DOUT2 (pyfirmata.pyfirmata.Pin)  = 9     : corrente na saída AC digital 2     
            * AC_DOUT3 (int)                        = 22    : saída AC dígital 3  (Fase CN18:2 Neutro CN18:1)   
            * I_AC_DOUT3 (pyfirmata.pyfirmata.Pin)  = 8     : corrente na saída AC digital 3       
         
        CONETOR CN16
            
            * AC_DIN0 (pyfirmata.pyfirmata.Pin) = 41 entrada digital AC 0 (Fase CN16:1 Neutro CN16:2)
            * AC_DIN1 (pyfirmata.pyfirmata.Pin) = 40 entrada digital AC 1 (Fase CN16:3 Neutro CN16:4)
            * AC_DIN2 (pyfirmata.pyfirmata.Pin) = 39 entrada digital AC 2 (Fase CN16:4 Neutro CN16:6)
            * AC_DIN3 (pyfirmata.pyfirmata.Pin) = 38 entrada digital AC 3 (Fase CN16:7 Neutro CN16:8)

        CONETOR CN15 (CN15:1 DC+ e CN15:10 DC-)
                
            * DC_DOUT1 (int) = 37 saída DC dígital 1  (CN15:2)
            * DC_DOUT2 (int) = 36 saída DC dígital 2  (CN15:3)
            * DC_DOUT3 (int) = 34 saída DC dígital 3  (CN15:4)
            * DC_DOUT4 (int) = 35 saída DC dígital 4  (CN15:5)
            * DC_DOUT5 (int) = 33 saída DC dígital 5  (CN15:6)
            * DC_DOUT6 (int) = 32 saída DC dígital 6  (CN15:7)
            * DC_DOUT7 (int) = 31 saída DC dígital 7  (CN15:8)
            * DC_DOUT8 (int) = 30 saída DC dígital 8  (CN15:9)
            obs: saídas pin 34 e 35 estão invertidas no hardware em relação ao silk
...
<mas código>
...
        
            * TECLA4 (pyfirmata.pyfirmata.Pin) = 11 acionamento da tecla 4
            * LED1  (int) = 12: led da tecla 1
            * LED2  (int) = 13: led da tecla 2
            * LED3  (int) = 14: led da tecla 3
            * LED4  (int) = 15: led da tecla 4
            * V_DOUTS (pyfirmata.pyfirmata.Pin) = 10: tensão das saídas digitais
            * V_INPW (pyfirmata.pyfirmata.Pin) = 11: tensão de entrada da fonte         

    METODOS
    """
    
 
    def __init__(self) -> None:
        self.nome=None



    def configura(self,portaCom,posJumpers) -> None:
        """
        Define a porta COM do computador a ser usada com a Jiga e indica ao software a posição
        física dos jumpers 

        Parameters

            * portacom: Número da porta COM
            * posJumpers:string de posição dos Jumpers

        Returns

            * None

        Exemplo

            * configura('COM2','0000000000011111')

        .. note::
            No hardware existe um posicionamento de jumpers que afeta se são usadas saídas ou entradas
            determinadas da placa. Ver diagrama elétrônico. Em resumo são

                * posJumpers = S5/S6+S7/S8+S9/S10+S11/S12='0000'+'0000'+'0000'+'0000' =000000000000

            sendo o valor 0 o jumper da esquerda em ON e o da direita em OFF e valor 1 contrario, por exemplo
            S5/S6 = 0101 siginifica 
        
            +-------+---------------+----------------+
            | Valor |  PosJumper_S5 |   PosJumper_S6 |
            +=======+=======+=======+=======+========+
            |bit    |  ON   |  OFF  |  ON   |  OFF   |
            +-------+-------+-------+-------+--------+
            |  0    |   x   |       |       |     x  |
            +-------+-------+-------+-------+--------+
            |  1    |       |    x  |    x  |        |
            +-------+-------+-------+-------+--------+        
            |  0    |   x   |       |       |     x  |
            +-------+-------+-------+-------+--------+
            |  1    |       |   x   |    x  |        |
            +-------+-------+-------+-------+--------+

            variável indexJumper posição 0 a 3

            +------------+------------+------------+------------+------------+
            |   Jumper   |      0     |      1     |      2     |     3      |
            +============+============+============+============+============+
            |     S5     |    DC_PW1  |   DC_PW2   |   SEL_BAT  |    NA      |
            +------------+------------+------------+------------+------------+
            |     S6     |    AC_PW1  | AC_SEL_PW1 |    AC_PW2  | AC_SEL_PW2 |
            +------------+------------+------------+------------+------------+

            
            variável indexJumper posição 4 a 7

            +------------+------------+------------+------------+------------+
            |   Jumper   |      4     |      5     |      6     |     7      |
            +============+============+============+============+============+
            |     S7     |   AC_DIN0  |   AC_DIN1  |   AC_DIN2  |  AC_DIN3   |
            +------------+------------+------------+------------+------------+
            |     S8     |  DC_DIN13  |  DC_DIN14  |  DC_DIN15  |  DC_DIN16  |
            +------------+------------+------------+------------+------------+

            variável indexJumper posição 8 a 11

            +------------+------------+------------+------------+------------+
            |   Jumper   |      8     |      9     |     10     |    11      |
            +============+============+============+============+============+
            |     S9     |  AC_DOUT3  |  AC_DOUT2  |  AC_DOUT1  |  AC_DOUT0  |
            +------------+------------+------------+------------+------------+
            |     S10    | DC_DOUT16  | DC_DOUT15  | DC_DOUT14  | DC_DOUT13  |
            +------------+------------+------------+------------+------------+

            variável indexJumper posição 12 a 15

            +------------+------------+------------+------------+------------+
            |   Jumper   |     12     |     13     |     14     |    15      |
            +============+============+============+============+============+
            |     S9     |   V_DOUTS  |   V_INPW   |  I_DC_PW1  |  I_DC_PW2  |
            +------------+------------+------------+------------+------------+
            |     S10    | I_AC_DOUT0 | I_AC_DOUT1 | I_AC_DOUT2 | I_AC_DOUT3 |
            +------------+------------+------------+------------+------------+

        """        
        self.posJumpers=posJumpers
        indexJumper=bytes(self.posJumpers,'utf-8')
        #Verifica que a variável que define os Jumpers esteja certa
        if len(indexJumper)!=16:
            raise Exception("numero de bits da string binaria diferente de 16")
        for item in indexJumper:    
            if item != 48:
                if item!=49:
                    raise Exception("string deve representar um numero binario 16 bits")

       
        self.DAQ = ArduinoMega(portaCom)  
        self.vutil = util
        self.it = self.vutil.Iterator(self.DAQ)
        self.it.start()


        # #DEFINIÇÃO DE PINOS DE SAÍDAS DIGITAIS AC E ENTRADAS ANALÓGICAS DE CORRENTE
        # # CONETOR CN18
        # self.AC_DOUT0     = 25    definido junto à SAÍDAS DIGITAIS DC - CONETOR CN11
        # self.I_AC_DOUT0   = self.DAQ.get_pin('a:11:i')    definido junto à PINOS BATERIA 12/24 - CONETOR CN8 E CN9
        # self.AC_DOUT1     = 24    definido junto à SAÍDAS DIGITAIS DC - CONETOR CN11
        # self.I_AC_DOUT1   = self.DAQ.get_pin('a:10:i') definido junto à PINOS BATERIA 12/24 - CONETOR CN8 E CN9          
        # self.AC_DOUT2     = 23    definido junto à SAÍDAS DIGITAIS DC - CONETOR CN11
        # self.I_AC_DOUT2   = self.DAQ.get_pin('a:9:i')  definido junto à PINOS POWER DC1 - CONETOR CN5      
        # self.AC_DOUT3     = 22    definido junto à SAÍDAS DIGITAIS DC - CONETOR CN11   
        # self.I_AC_DOUT3   = self.DAQ.get_pin('a:8:i')   definido junto à PINOS POWER DC2 - CONETOR CN6

        # #DEFINIÇÃO DE PINOS DE ENTRADAS DIGITAIS AC 
        # # CONETOR CN16

...
<mas código>
...

        if indexJumper[11]==48:            
            self.AC_DOUT0      = 25            
            self.DC_DOUT13     = None
        elif indexJumper[11]==49:            
            self.DC_DOUT13     = 25
            self.AC_DOUT0      = None          

        if indexJumper[10]==48:            
            self.AC_DOUT1      = 24
            self.DC_DOUT14     = None
        elif indexJumper[10]==49:            
            self.DC_DOUT14     = 24  
            self.AC_DOUT1      = None          

        if indexJumper[9]==48:            
            self.AC_DOUT2      = 23
            self.DC_DOUT15     = None
        elif indexJumper[9]==49:            
            self.DC_DOUT15     = 23 
            self.AC_DOUT2      = None             

        if indexJumper[8]==48:            
            self.AC_DOUT3      = 22
            self.DC_DOUT16     = None
        elif indexJumper[8]==49:            
            self.DC_DOUT16     = 22 
            self.AC_DOUT3      = None       
         

        #DEFINIÇÃO DE COMUNICAÇÃO
        # CONETOR CN12
        # TO DO:

        #DEFINIÇÃO DE PINOS DE ENTRADAS DIGITAIS DC - BARRAMENTO 1 
        # CONETOR CN14
        self.DC_DIN1 = self.DAQ.get_pin('d:53:i')   
        self.DC_DIN2 = self.DAQ.get_pin('d:52:i')
        self.DC_DIN3 = self.DAQ.get_pin('d:51:i')
        self.DC_DIN4 = self.DAQ.get_pin('d:50:i')
        self.DC_DIN5 = self.DAQ.get_pin('d:49:i')
        self.DC_DIN6 = self.DAQ.get_pin('d:48:i')
        self.DC_DIN7 = self.DAQ.get_pin('d:47:i')
        self.DC_DIN8 = self.DAQ.get_pin('d:46:i')

        #DEFINIÇÃO DE PINOS DE ENTRADAS DIGITAIS DC - BARRAMENTO 2 
        # CONETOR CN13
        self.DC_DIN9 = self.DAQ.get_pin('d:45:i')
        self.DC_DIN10 = self.DAQ.get_pin('d:44:i')
        self.DC_DIN11 = self.DAQ.get_pin('d:43:i')
        self.DC_DIN12 = self.DAQ.get_pin('d:42:i')

        if indexJumper[4]==48:            
             self.AC_DIN0 = self.DAQ.get_pin('d:41:i')
             self.DC_DIN13 =None
        elif indexJumper[4]==49:                        
            self.DC_DIN13 = self.DAQ.get_pin('d:41:i')
            self.AC_DIN0 = None

```

</details> 


<details>
  <summary><b>📜 Ver ejemplo del código de la API ESP32-Modbus en lenguaje de la IDE de Arduino </b>></summary>
 
```C


//  *** ModbusIP object ***
ModbusIP mb;

...
<mas código>
...
  
//************************************************************************************
// @BRIEF: setup
// @PARAM none
// @RETURN: none
void setup() {
...
<mas código>
...

  // MODBUS SERVER CONFIGURATION
  mb.server();

 //Register criation and initial values for coil reg. map D_IO00 to D_IOxF type
  
  mb.addCoil(CL_VAL_D_O00);
  mb.Coil(CL_VAL_D_O00,false);

  mb.addCoil(CL_VAL_D_O01);
  mb.Coil(CL_VAL_D_O01,false);

  mb.addCoil(CL_VAL_D_O02);
  mb.Coil(CL_VAL_D_O02,false);

  mb.addCoil(CL_VAL_D_O03);
  mb.Coil(CL_VAL_D_O03,false);

  ...
<mas código>
...
  
  //Register criation and initial values for input reg. map D_IO00 to D_IOxF type
  
  mb.addIreg(IR_TYPE_D_IO00);
  mb.Ireg(IR_TYPE_D_IO00,0x00);

  mb.addIreg(IR_TYPE_D_IO01);
  mb.Ireg(IR_TYPE_D_IO01,0x00);
  
  mb.addIreg(IR_TYPE_D_IO02);
  mb.Ireg(IR_TYPE_D_IO02,0x00);
  
  
  //Register criation and initial values for analow pwm output 

  mb.addHreg(HR_APWM_OUT_LEVEL); //Holding Register for GPI mapping and level
  mb.Hreg(HR_APWM_OUT_LEVEL,0x000); //0xXYYY; X = 0,1,2..15 (0:none, 1..15: GPO mapping); YYY = 0,...,FF (PWM level)

  mb.addIreg(IR_APWM_OUT_LEVEL); //Input Register for GPI mapping and level
  mb.Ireg(IR_APWM_OUT_LEVEL,0x000); // 0xXYYY; X = 0,1,2..15 (0:none, 1..15: GPO mapping); YYY = 0,...,FF (PWM level)

  ...
<mas código>
...

//************************************************************************************
// @BRIEF: GPIO write analog PWM
// @PARAM int val: 0xXYYY, X is the pin (as mapping) , YYY = 0,...,255 (PWM level)
// @RETURN: bool sucess: true or false   

bool write_APWMDO(int val) {
  bool sucess=true;
  char StringVal[8];
  sprintf(StringVal,"%03x", val);
  char pin=StringVal[0];
  String state=String(StringVal);
  state=state.substring(1);
  //state= "0x"+state;
  char charArray[2];
  state.toCharArray(charArray,state.length() + 1);
  int answer = strtol(charArray, NULL, 16);
  
  switch (pin) {
    case '0':
      analogWrite(D_IO00, answer);
      break;
    case '1':
      analogWrite(D_IO01, answer);
      break;
 
  ...
<mas código>
...

//************************************************************************************
// @BRIEF: loop
// @PARAM none
// @RETURN: none
void loop() {

  ...
<mas código>
...

  //start task
  mb.task();

  // Change register values to configurate GPIO as input, output or input_pullup 
  for (int i=0; i<=0xF; i++){ 
    if  (mb.Hreg(i+0x10) != mb.Ireg(i+0x3F8)) {
      mb.Ireg(i+0x3F8,mb.Hreg(i+0x10));
     Config_DIO(i,mb.Ireg(i+0x3F8));  
    };
  };

  ...
<mas código>
...

```

</details> 

<details>
  <summary><b>📜 Aplicación </b>></summary>

![Paneles](https://drive.google.com/uc?export=view&id=1RXv_XtWBBSXE_-u39rQp9afaiXxkXpOF)

</details>

--

<!-- QUINTO PROYECTO -->

## 2022
### Grabación y control de calidad de placas electrónicas

Esta aplicación  grava microcontroladores STMicroelectronics y através de un hardware personalizado realiza un ensayo que identifica defectos en la producción de placas electrónicas. 

**Caracteristicas:**  
- Lenguaje [![Lenguaje labview](https://img.shields.io/badge/NI-Labview-blue?logo=labview&logoColor=white)](https://www.ni.com/es/shop/labview.html)

**Hardware:**  

- Personalizado  desarrollado por el cliente


<details>
  <summary><b>📜 Ver ejemplo del código en labview </b>></summary>
 
 ![Snipped labview](https://drive.google.com/uc?export=view&id=1eq2ARQ8EnMts_C7aP2tix-5ZTqGg9tOM)


</details> 


<details>
  <summary><b>📜 Aplicación </b>></summary>

![Monitoreo remoto](https://drive.google.com/uc?export=view&id=1gOmprDDvN5PKs5ydAp5ZWZYX6YLsWseq)

</details>

--

<!-- SEXTO PROYECTO -->

## 2021
### Interface HMI para reator químico

Esta aplicación  es una interface para visualización de un reactor químico de laboratório

**Caracteristicas:**  
- Construcción en ambiente DOPSoft 
- Comunicación modbus RTU sobre red 485

**Hardware:**  

- Controladores Delta
- Servomotor con drive Delta


<details>
  <summary><b>📜 Ver ejemplo del código sintaxe DELTA DOPSoft </b>></summary>

```python

# STATUS BUTTON START TEMPERATURE LOOP
# BUTTON OFF
IF [TEMP_OPER] !=2 
	#CHECK VALVE OUTPUT (MANUAL OR AUTO)
	[TEMP_VALVE_OUT]=[TEMP_VALVE_OUT_LOCAL]
	# LOCAL VARIAVEL FOR EFFECT COOLING BAR
	[TEMP_REACTOR_MV_LOCAL] = 0 -([TEMP_REACTOR_MV]) (SIGNED)
	#VISIBILITY SWITCH VALVE COOLING
	BITON([TEMP_AUX2])
	#WHEN ERROR SWITCH TO MANUAL
	# TEMPERATURE REACTOR HIGH
	IF [TEMP_RLY_REACTOR]!=0
		# TEMPERATURE JACKET HIGH
		IF [TEMP_RLY_JACKET] != 0
			#PRESSURE HIGH
			IF [PRESS_RLY_REACTOR] != 0
				#NO ERROR AUTO
				[TEMP_OPER] =0
			ELSE
				#IF ERROR GO TO MANUAL
				[TEMP_OPER] =1
				[TEMP_REACTOR_MV]=0
			ENDIF
		ELSE
			#IF ERROR MANUAL
			[TEMP_OPER] =1
			[TEMP_REACTOR_MV]=0
		ENDIF
	ELSE
		#IF ERROR MANUAL
		[TEMP_OPER] =1
		[TEMP_REACTOR_MV]=0		
	ENDIF
ELSE
	#CHECK VALVE OUTPUT MANUAL (FOR ENABLE COOLING))
	TEMP_VALVE_OUT = 0
	#VISIBILITY SWITCH VALVE COOLING
	BITOFF([TEMP_AUX2])
	# LOCAL VARIAVEL FOR EFFECT COOLING BAR = 0
	[TEMP_REACTOR_MV_LOCAL] = 0
	# TEMPERATURE SP SECURITY
	[TEMP_REACTOR_SP] = 30 

ENDIF

 ```

</details> 


<details>
  <summary><b>📜 Aplicación </b>></summary>

![Monitoreo remoto](https://drive.google.com/uc?export=view&id=1JHPFmBLdXw5FTEFd9--9dlMDq6F1rHc4)

</details>

--

<!-- SEPTIMO PROYECTO -->

## 2016
### RGB VIEW

Esta es una aplicación basada en procesamiento de imagen, desarrollada para o laboratório NQTR de la Universidad Federal de Rio de Janeiro para investigación de cineticas de precipitación de partículas. 

**Caracteristicas:**  
- Lenguaje [![Lenguaje labview](https://img.shields.io/badge/NI-Labview-blue?logo=labview&logoColor=white)](https://www.ni.com/es/shop/labview.html)

**Hardware:**  

- Camara acoplada al computador
- Sistema de actuación basado en arduino.


<details>
  <summary><b>📜 Ver ejemplo del código en labview </b>></summary>
 
 ![Snipped labview](https://drive.google.com/uc?export=view&id=1dXMsCr-8BvqAHmRtc1imyW0koUU-7Nnf)


</details> 


<details>
  <summary><b>📜 Aplicación </b>></summary>

![RGBView](https://drive.google.com/uc?export=view&id=16_ZAgzym4sGcVUp-OS1VVTw36bZNrL1a)


</details>

--

## 2013
### CAMPO ELÉCTRICO CRÍTICO

Esta es una aplicación para lectura de variables electricas e la determinacion de campos electricos en celulas de ensayo de emulsioes óleo agua

**Caracteristicas:**  
- [![Lenguaje Pascal / Delphi](https://img.shields.io/badge/Pascal-Delphi-blue?logo=delphi&logoColor=white)](https://www.embarcadero.com/br/products/delphi)

- Protocolo de comunicación SCPI (Standard Commands for Programmable Instruments)

**Hardware:**  

- [![Fuente de mediciones dinámicas Agilent](https://img.shields.io/badge/Agilent-6634B-blue)](https://www.keysight.com/find/6634B)
- [![Picoamperímetro Keithley](https://img.shields.io/badge/Keithley-6487-blue)](https://www.tek.com/en/datasheet/series-6400-picoammeters/6487-picoammeter-voltage-source)




<details>
  <summary><b>📜 Ver ejemplo del código en pascal </b>></summary>
 
 ```Pascal

procedure TfrmAgilent.btnIniciarClick(Sender: TObject);
var
frameEstatus:string;
tensao:string;
begin
  if portaAgilent.Connected=false then
    begin
      portaAgilent.Connected:=true;
      portaAgilent.ClearBuffer(true,true);
      timerProgresso.Enabled:=true;
    end
  ;
  btnIniciar.Enabled:=false;
  btnParar.Enabled:=true;
  btnExportar.Enabled:=false;
  btnRampaPatamar.Enabled:=false;
  Tabsheet3.Enabled:=false;

  portaAgilent.WriteStr('*RST'+#10);
  sleep(200);
  portaAgilent.WriteStr('*CLS'+#10);
  sleep(200);


  frameEstatus:= 'OUTPUT:STATE ON;STATE?'+#10;
  portaAgilent.WriteStr(frameEstatus);
  sleep(200);
  tempoInicial:=time;
  tensao:='SOUR:VOLT '+floattostr(vetorTensao[0])+#10;
  portaAgilent.WriteStr(tensao);
  Timer.Enabled:=true;
  iTempo:=0;
  Series1.AddXY(vetorTempo[0],vetorTensao[0]);
  iLed:=0;

end;

procedure TfrmAgilent.btnPararClick(Sender: TObject);
var
frameEstatus:string;
begin
 if portaAgilent.Connected=true then
  begin
    frameEstatus:= 'OUTPUT:STATE OFF'+#10;
    portaAgilent.WriteStr(frameEstatus);
    portaAgilent.Connected:=false;
    led1.Active:=false;
    led2.Active:=false;
    led3.Active:=false;
    Timer.Enabled:=false;
    iTempo:=0;
    btnParar.Enabled:=false;
    btnRampaPatamar.Enabled:=true;
    Tabsheet3.Enabled:=true;
    timerProgresso.Enabled:=false;
    iLed:=0;
    btnExportar.Enabled:=true;
  end
 ;

end;

procedure TfrmAgilent.datapackAgilentPacket(Sender: TObject;
  const Str: String);
  var
  tempoTrascorrido:integer;
  straux:string;
begin
    if (str<>'1') and (str<>'0') then
      begin
        straux:=copy(Str,2,length(Str)-1);
        dsAmperagem.Value:=strtofloat(straux)*1000;
        tempoAtual:=time;
        tempoTrascorrido:=round((TimeStampToMSecs(DateTimeToTimeStamp(tempoAtual))-
                    TimeStampToMSecs(DateTimeToTimeStamp(tempoInicial)))/1000);

        Series2.AddXY(tempoTrascorrido,dsAmperagem.Value);
        Series2.RefreshSeries;
      end
    ;
end;

```


</details> 


<details>
  <summary><b>📜 Aplicación </b>></summary>

![CEC](https://drive.google.com/uc?export=view&id=14mUEc7MtIwKq_nxcBaninE5e5dXX1Wm9)

</details>

--

## OTROS PROYECTOS
- 2019 e-Trasmisor realizando medidas de presión de un transmisor diferencial marca Yokogawa - Lenguaje: labview
- 2017 Interfaces para ultrafreezer -90º marca Coldlab - Lenguaje de DOPSoft Delta
- 2015 Medidor de turbidez para registro de datos de un turbidímetro marca Mettler Toledo - Lenguaje: labview
- 2014 a 2021 - Interfaces para biorreactores marca Biofoco - Lenguaje de DOPSoft Delta
- 2013 e-Biostation (coautor) para monitoramento y control de Biorreactores - Lenguaje: pascal/delphi
- 2003 - 2019 Diversos Scripts e interfaces GUI para estudio y enseñanza de control de procesos - Lenguaje: matlab
- 2003 Sistema de monitoreo y control de digestores anaeróbios - Lenguaje: pascal/delphi
- 1999 Interface de control de reactor catalítico en un grupo de investigación de la UdeA - Lenguaje: labview
