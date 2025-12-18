# DuckPro
Proyecto de Fundamentos de Programación Orientada a Eventos

Autoría de: 
María Fernanda González Ramírez.
Tercer semestre de ingeniería de sistemas - Universidad del Valle sede Tuluá

--Descripción del proyecto--

Este proyecto es una aplicación de escritorio diseñada para simular una carrera de patos, desarrollado en el lenguaje Java, haciendo uso de Swing.
El sistema permite registrar participantes (Tanto los concursantes como sus patos), crear y validar carreras (Además de guardar sus resultados), simular visualmente una carrera animada y generar estadísticas básicas de los datos que han participado en carreras.
Este proyecto fue diseñado siguiendo el patrón Modelo-Vista-Controlador, también conocido por sus siglas MVC.
Se hizo uso de Java Swing, Java, JOptionPane y Timer (javax.swing), además de librerías para el manejo de archivos planos (.txt).

--Funciones principales--

- Registro de participantes.
Los participantes deben de registrarse con nombre, edad, documento y categoría, además del nombre del pato.
En la sección de registro, se pueden ver los participantes ya registrados.

- Búsqueda de participantes.
Por medio de JOptionPane, se puede hacer búsqueda de los participantes por medio de su documento o su nombre, y el programa arrojará todos sus datos.

- Carreras.
Para iniciar una carrera, se seleccionan tres patos por sus nombres. No se pueden repetir nombres de los patos, los tres patos tienen que estar registrados y deben pertenecer a la misma categoría. La carrera inicia si y solo si las condiciones se cumplen.

- Simulación.
En pantalla se ve la simulación de la carrera de patos. Los resultados son completamente aleatorios, el desplazamiento depende completamente de un Random incorporado al código.
Una vez concluida la carrera, en pantalla, mediante un JOptionPane.showMessageDialog, se muestra el podio (Primero, segundo, tercer lugar).

- Estadísticas.
En el menú, se encuentra un botón de estadísticas que, al accionar, abre un JOptionPane que muestra el nombre de los patos que han participado en carreras, sus carreras ganadas (En primer puesto) y las carreras en las que han participado.

- Resultados de las carreras.
Los resultados se guardan en un archivo llamado "resultados.txt" en el que se almacena el nombre de la carrera, fecha, categoría y podio final.

- Arquitectura del proyecto.
Modelo: App, Carrera, EstadisticaPato, Participante.
Vista: CarreraAnimForm, CrearCarreraForm, MenuForm, RegistroForm.
Controlador: MainControlador.

- ¿Cómo ejecutarlo?
Se abre el peograma en un IDE compatible con Java, y se ubica en el archivo App, donde se ejecuta.
Tener en consideración la configuración del JDK.

- Ejemplo de uso.
Ejecutar App → Registrar participantes con sus respectivo patos → Crear una carrera seleccionando tres patos → Validar la carrera → Iniciar la simulación → Visualizar el podio → Consultar estadísticas en el menú.



