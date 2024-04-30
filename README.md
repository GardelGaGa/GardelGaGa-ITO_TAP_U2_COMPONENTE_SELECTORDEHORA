# SELECTOR DE HORA

## Descripción:

Este componenete Java proporciona a los usuarios la capacidad de seleccionar y establecer la hora de manera intuitiva a través de una interfaz gráfica. Está diseñado para su integración sencilla en aplicaciones `Java Swing`, pudiendo ser fácilmente agregado a `JFrame` u `JDialog`.

El componente principal consta de dos clases principales: `TimePanel` y `TimeChooser`, que trabajan en conjunto para permitir a los usuarios seleccionar la hora deseada y gestionar su interacción con el componente de forma visual.

TimePanel presenta una interfaz gráfica que muestra la hora actual y proporciona controles visuales para ajustarla, mientras que TimeChooser facilita la integración del panel de selección de tiempo en aplicaciones existentes.

Con su diseño modular y uso de componentes estándar de Swing, este componente ofrece una manera conveniente y segura de gestionar la selección de tiempo en aplicaciones Java, mejorando así la experiencia del usuario.

## Usos:
1. **Aplicaciones de Gestión de Citas y Calendarios:** Este componente puede integrarse en sistemas de gestión de citas y calendarios donde se necesite la selección y establecimiento precisos de la hora para programar eventos, reuniones o citas.
2. **Herramientas de Programación y Planificación:** Puede ser utilizado como parte de herramientas de programación y planificación que requieran la entrada de tiempo por parte del usuario, como aplicaciones de gestión de proyectos, herramientas de seguimiento del tiempo o planificadores de tareas.
3. **Aplicaciones de Reservas y Programación de Recursos:** Integración en aplicaciones de reservas y programación de recursos, como sistemas de reservas de citas en línea, gestión de salas de reuniones, programación de recursos en instalaciones deportivas, entre otros.
4. **Mejora de la Experiencia del Usuario en Aplicaciones de Productividad:** Proporciona una forma intuitiva para que los usuarios seleccionen la hora deseada, mejorando la experiencia del usuario en aplicaciones de productividad como suites de oficina, gestores de tareas o aplicaciones de gestión del tiempo.
5. **Personalización de Sistemas de Gestión Empresarial:** Puede ser integrado en sistemas de gestión empresarial personalizados para ofrecer a los usuarios una forma fácil y rápida de ingresar la hora en formularios de entrada de datos, como en sistemas de gestión de recursos humanos, sistemas de gestión de inventario, etc.




## Características:
- Generación de horas seleccionables de manera intuitiva y personalizable.
- Integración sencilla con cualquier componente Swing (`JFrame`, `JDialog`) para una experiencia de usuario fluida.
- Interfaz gráfica de arrastrar y soltar para una manipulación fácil y eficiente en interfaces gráficas.


## Requisitos:
- Entorno de ejecución Java (JRE)
- Bibliotecas Swing
- Plataforma compatible
- Interfaz gráfica

## API
### TimePanel

#### Descripción
La clase TimePanel es un panel de Swing que permite a los usuarios seleccionar y ajustar la hora, los minutos y AM/PM. Proporciona una interfaz gráfica para que los usuarios establezcan la hora deseada.

#### Campos:
| Tipo| Campo| Descripción|
|---------------|----------|-----------------------------------------------------------------------------------------------|
| `Calendar`| `cal`| Almacena la instancia de Calendar que representa la hora actual del sistema.|
| `JTextField`| `texto`| Almacena una referencia al campo de texto donde se mostrará la hora seleccionada.|
| `JLabel`| `Hora`| Muestra la hora seleccionada por el usuario en formato de 12 horas.|
| `JLabel`| `Minuto`| Muestra los minutos seleccionados por el usuario.|
| `JLabel`| `AmPm`| Muestra si es AM o PM.|
| `JLabel`| `btnCancel`| Botón para cancelar la selección de hora.|
| `JLabel`| `btnSet`| Botón para confirmar y establecer la hora seleccionada.|

#### Métodos:
| Nombre| Tipo de Dato que Retorna | Tipo de dato que Recibe | Descripción|
|-------|--------------------------|-------------------------|------------|
| `ajustarHora`| `void`| `String`| Ajusta la hora seleccionada según el valor recibido ('+' para aumentar, '-' para disminuir).|
| `ajustarMinuto`| `void`| `String`| Ajusta los minutos seleccionados según el valor recibido ('+' para aumentar, '-' para disminuir).|  
| `initComponents`| `void`| `N/A`| Inicializa y configura los componentes de la interfaz gráfica.|

### Clase: TimeChooser

#### Descripción
La clase TimeChooser es un campo de texto personalizado que permite a los usuarios seleccionar la hora utilizando un panel de selección de tiempo. Facilita la entrada y visualización de la hora en aplicaciones Java.

#### Campos:
| Tipo| Campo| Descripción|
|-----|------|------------|
| `Dimension`| `dimension`| Almacena las dimensiones del componente.|
| `JButton`| `button`| Botón para abrir el panel de selección de tiempo.|
| `JPopupMenu`| `popup`| Menú emergente que contiene el panel de selección de tiempo.|
| `TimePanel`| `timePanel`| Panel de selección de tiempo que se muestra en el menú emergente.|

#### Métodos:
| Nombre| Tipo de Dato que Retorna| Tipo de dato que Recibe| Descripción|
|-------|-------------------------|------------------------|------------|
| `updateButton`| `void`| `N/A`| Actualiza la dimensión y posición del botón de apertura del panel de selección de tiempo.|
| `componentResized`| `void` | `ComponentEvent`| Ajusta el botón cuando el componente cambia de tamaño.|
| `componentMoved`| `void`| `ComponentEvent`| Método vacío llamado cuando el componente se mueve.|
| `componentShown`| `void`| `ComponentEvent`| Método vacío llamado cuando el componente se muestra.|
| `componentHidden`| `void`| `ComponentEvent`| Método vacío llamado cuando el componente se oculta.|

## Instalación
Para utilizar este componente en tu proyecto, sigue estos pasos:

1. Obtener el repositorio


 ```bash
      git clone https://github.com/GardelGaGa/GardelGaGa-ITO_TAP_U2_COMPONENTE_SELECTORDEHORA.git
   ```

   Otra opción es descargar `ZIP`.
   ![image](https://github.com/GardelGaGa/GardelGaGa-ITO_TAP_U2_COMPONENTE_SELECTORDEHORA/assets/69336597/047503ff-f5ed-4759-ac5c-26c2a78a554b)

2. Importa el proyecto en tu IDE preferido (NetBeans o VS code).

3. Asegúrate de que el proyecto se compila sin errores para crear el `.jar` según la versión de tu Java.

## Uso
1. Compila tu proyecto para crear el archivo `.jar`

  ![image](https://github.com/GardelGaGa/GardelGaGa-ITO_TAP_U2_COMPONENTE_SELECTORDEHORA/assets/69336597/ee41794b-bf32-4bdc-bd25-3323010fafde)

   Posteriormente presiona `SHIFT + F11` o clikea en este boton 
   ![image](https://github.com/GardelGaGa/GardelGaGa-ITO_TAP_U2_COMPONENTE_SELECTORDEHORA/assets/69336597/cd68b0af-0546-4fab-bb0c-ce065fe12a04)

añadiremos a nuestra categoria



2. Agrega el componente a tu paleta de componentes. Da click derecho en **Tools** en la barra de tareas y despues da click en **Swing/AWT Components** para abrir el **Palette Manager**
   
![image](https://github.com/GardelGaGa/GardelGaGa-ITO_TAP_U2_COMPONENTE_SELECTORDEHORA/assets/69336597/b5212882-1ce9-4e93-8609-ad40591494a3)

Una vez abierto este cuadro damos click en  **Add from JAR** para seguir con el proceso 

![image](https://github.com/GardelGaGa/GardelGaGa-ITO_TAP_U2_COMPONENTE_SELECTORDEHORA/assets/69336597/4b9f39f0-72fe-4dbb-a4ac-2ca19713532b)

Navega hasta la carpeta **dist** del proyecto y selecciona `jar`

![image](https://github.com/GardelGaGa/GardelGaGa-ITO_TAP_U2_COMPONENTE_SELECTORDEHORA/assets/69336597/14b250c8-e172-46ab-937e-cbb554d83ce6)

![image](https://github.com/GardelGaGa/GardelGaGa-ITO_TAP_U2_COMPONENTE_SELECTORDEHORA/assets/69336597/663164f0-3a14-4720-aa40-1098196ef3d9)

Seleccionamos a que categoria añadimos nuestra nueva herramienta 

![image](https://github.com/GardelGaGa/GardelGaGa-ITO_TAP_U2_COMPONENTE_SELECTORDEHORA/assets/69336597/0b90417d-6e4a-4088-bdea-1c10cd9022ff)

3. Ya está listo para usar y arrastrar a tus componentes



## Funcionamiento
¡Descubre cómo funciona este componente visual *Selector de hora*!
Haz clic para ver el video ahora mismo ---> 


## Contribuir
Si deseas contribuir a este proyecto, por favor sigue los siguientes pasos:
1. Haz un fork del repositorio.
2. Crea una nueva rama para tu característica o corrección de errores.
3. Haz tus cambios.
4. Envía un pull request.



## Autores
- Santos Perez Valentino Gardel - *Estudiante del ITO* - [Contacto]([GardelGaGa (github.com)](https://github.com/GardelGaGa))
  
- Alary Guzmán Jiménez - *Estudiante del ITO* - [Contacto]([AlaryGuzman (github.com)](https://github.com/AlaryGuzman))




## Agradecimientos
- Gracias a todos los que contribuyeron a este proyecto!
- A mi gato por acompañarme en las noches de desvelo .













