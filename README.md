# tcpdump-commands
# tshark-commands
# commands
![image](https://byte-mind.net/wp-content/uploads/2019/08/tcpdump-logo-450x410.jpg)
![image](https://media.licdn.com/dms/image/v2/D5612AQHPO-2Iu-iP0w/article-cover_image-shrink_600_2000/article-cover_image-shrink_600_2000/0/1659802184384?e=2147483647&v=beta&t=P_nvKbQr042i9jw4JPCbrPVRKAWnyFQR1yPT0kBqiPc)


-[<tcpdump -w {interfaz} <another-commands>][Description: "Este comando sirve para guardar las capturas de datos en un archivo!"]

-[<tcpdump -i  {interfaz} any <another-commands>][Description: "Este comando es utilizado para capturar paquetes en cualquier interfaz!"]

-[<tcpdump   -ni {interfaz}   <another-coommands>][Description: "Este comando sirve para Desactivar la resolucion de nombres!"],

-[<tcpdump -c {interfaz} <another-commands>][Description: "Este comando sirve para limitar el numero de paquetes a capturar o interceptar!"]

-[<tcpdump -i {interfaz} any not port 22{SSH} or 23{Telnet} <another-commands>][Description: "Si quieres guardar capturas de datos en cualquier interfaz pero excluyendo SSH/Telnet!"]


tcpdump@commands, todos los comandos de tcpdump, e iré agregando unos cuantos de tshark, y su funcionamiento detrás de sus capturas de datos, esta guia es para uso personal
Estoy desarrollando una guía personal sobre el uso de tcpdump, una herramienta fundamental en el análisis y monitoreo del tráfico de red. Esta guía no solo recopila los comandos esenciales que utilizo frecuentemente, sino que también explica cómo funciona internamente cada uno, con el objetivo de comprender verdaderamente lo que ocurre detrás de cada captura.

tcpdump es una herramienta poderosa que permite observar el comportamiento real de una red en tiempo real. A través de ella, se pueden detectar problemas de conectividad, identificar tráfico sospechoso, diagnosticar fallos en servicios y comprender mejor la comunicación entre dispositivos y servidores. Lo interesante de trabajar con esta utilidad es que no se trata solo de ejecutar comandos, sino de entender cómo el sistema operativo interactúa con los paquetes, cómo se filtran mediante expresiones BPF, y cómo aprovechar todo esto para sacar conclusiones precisas.

Mi intención al documentar estos comandos no es solo tener una referencia técnica rápida para mi uso diario, sino también compartir conocimiento. Por eso, si tú también llegas a leer esto, siéntete con la total libertad de utilizar mis ejemplos y comandos. Estamos aquí para apoyarnos mutuamente y crecer como comunidad técnica.

Más adelante, iré incorporando comandos de tshark, que es la contraparte en consola de Wireshark, y permite un análisis aún más detallado de las capturas gracias a su capacidad de decodificar protocolos de forma profunda. La idea es que esta guía se convierta en una especie de bitácora técnica, personal pero útil, tanto para estudio como para tareas prácticas en redes, seguridad informática y administración de sistemas.


               Objetivos de esta guía

    Documentar los comandos de uso frecuente con ejemplos claros.

.Explicar el funcionamiento interno de cada acción ejecutada.

.Servir como referencia rápida para tareas de diagnóstico y análisis.

.Compartir el conocimiento de forma abierta con la comunidad técnica.

.Incluir más adelante comandos y usos de tshark como complemento avanzado de análisis en consola.

