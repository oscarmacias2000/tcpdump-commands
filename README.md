# tcpdump-commands
# tshark-commands
# commands
![image](https://byte-mind.net/wp-content/uploads/2019/08/tcpdump-logo-450x410.jpg)



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
    -i <interfaz>
    -ni <interfaz>
    -w <interfaz>
    -c <interfaz
    -i any <interfaz>
    -i any not port<22><23> <interfaz>
.Explicar el funcionamiento interno de cada acción ejecutada.

.Servir como referencia rápida para tareas de diagnóstico y análisis.

.Compartir el conocimiento de forma abierta con la comunidad técnica.

.Incluir más adelante comandos y usos de tshark como complemento avanzado de análisis en consola.


           Licencia y uso

Esta documentación es de uso personal, pero está publicada con el propósito de colaborar y aprender en conjunto. Puedes reutilizar, modificar o complementar el contenido libremente. Si te es útil, no dudes en adaptarlo a tus propias necesidades o contribuir con mejoras. La idea es ayudarnos mutuamente como profesionales y entusiastas del mundo de las redes.


        Sobre el enfoque técnico

Cada comando documentado en esta guía no solo se presenta como una instrucción aislada, sino que viene acompañado de una explicación de cómo se comporta internamente. Esto incluye aspectos como:

.La forma en que tcpdump accede a las interfaces de red mediante libpcap.

.Cómo se ejecutan los filtros BPF en el kernel para mejorar el rendimiento.

.La interpretación de los paquetes a nivel de protocolos (IP, TCP, UDP, etc.).

.La relación entre las capturas y herramientas gráficas como Wireshark.

.Este enfoque busca ir más allá de memorizar comandos, para realmente comprender el comportamiento de la red desde una perspectiva de bajo nivel.

        Próximamente: tshark-wireshark   

En etapas posteriores, se integrarán ejemplos y comandos clave de tshark, la versión CLI de Wireshark, que ofrece capacidades de análisis profundas y altamente configurables, ideales para automatización o análisis masivo de archivos .pcap.

        
