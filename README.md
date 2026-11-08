# Orbit OS | Orbit Terminal

### One terminal. Multiple systems. Endless possibilities.

**Plataforma experimental que combina hardware personalizado, electrónica, informática y un entorno de control desarrollado por Miguel Rodríguez Saiz dentro de Ardu Solutions.**

[![Version](https://img.shields.io/badge/Orbit_OS-1.0.0-2563EB?style=flat-square)](CHANGELOG.md)
![Status](https://img.shields.io/badge/Hardware-Prototype-F59E0B?style=flat-square)
![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-4-A22846?style=flat-square&logo=raspberrypi&logoColor=white)
![Windows](https://img.shields.io/badge/HP-Windows_10-0078D4?style=flat-square&logo=windows&logoColor=white)
![Python](https://img.shields.io/badge/Python-3-3776AB?style=flat-square&logo=python&logoColor=white)
![React](https://img.shields.io/badge/React-TypeScript-61DAFB?style=flat-square&logo=react&logoColor=black)
![Arduino](https://img.shields.io/badge/Arduino-Nano-00878F?style=flat-square&logo=arduino&logoColor=white)
![License](https://img.shields.io/badge/License-Apache--2.0-16A34A?style=flat-square)

**[Web oficial](https://ardu01.github.io/orbit-web/) · [Repositorio](https://github.com/ardu01/Orbit-OS) · [Portfolio](https://ardu01.github.io/proyectos/) · [Ardu Solutions](https://ardusolutions.pages.dev/)**

---

## 01. Introducción

**Orbit Terminal** es un proyecto experimental de ingeniería que combina dos plataformas informáticas dentro de una única estación de trabajo compacta.

Su diseño se basa en un terminal de sobremesa con carcasa personalizada, pantalla integrada, controles físicos e infraestructura electrónica propia.

El sistema combina un ordenador HP reutilizado, una Raspberry Pi 4 y diferentes dispositivos electrónicos, proporcionando una plataforma versátil para experimentación, desarrollo y control.

**Orbit OS** es el entorno de software desarrollado para gestionar la experiencia de usuario, supervisar los equipos conectados y centralizar las funciones del terminal.

El proyecto abarca diferentes disciplinas:

- Diseño mecánico y modelado CAD.
- Fabricación mediante impresión 3D.
- Electrónica y microcontroladores.
- Desarrollo de software.
- Sistemas Linux y Windows.
- Comunicación entre dispositivos.
- Interfaces de usuario.
- Automatización y control.

### Visión del proyecto

Orbit Terminal nace con el objetivo de construir una estación informática experimental que permita trabajar con diferentes sistemas y dispositivos desde una interfaz centralizada.

Su arquitectura busca aprovechar hardware existente, incorporar componentes electrónicos y facilitar la evolución modular del conjunto.

El propósito es disponer de una plataforma física para desarrollar, probar e integrar nuevas herramientas tecnológicas.

## 02. Orbit OS 1.0.0

**Orbit OS** es el entorno de control del terminal.

Su interfaz está diseñada para ofrecer una experiencia visual unificada, con una estética tecnológica oscura y acentos ámbar.

El sistema integra funciones de supervisión, navegación, gestión de dispositivos y control de las plataformas conectadas.

### Interfaz principal

![Inicio de Orbit OS](assets/screenshots/inicio_1920x1080.png)

*Captura original de la pantalla de inicio de Orbit OS 1.0.0, conservada del README del proyecto.*

La interfaz presenta información de los sistemas conectados, accesos rápidos y controles de funcionamiento.

### Características principales

- Panel centralizado de información.
- Estado de los sistemas conectados.
- Monitorización de hardware.
- Controles de funcionamiento.
- Herramientas de electrónica.
- Gestión de configuración.
- Integración con dispositivos externos.
- Interfaz optimizada para la pantalla del terminal.
- Funcionamiento con hardware real o simulación identificada.

## 03. Información general

| Campo | Información |
|---|---|
| Proyecto | Orbit Terminal |
| Software | Orbit OS |
| Desarrollador | Miguel Rodríguez Saiz |
| Organización | Ardu Solutions |
| Categoría | Hardware / Sistemas / Electrónica |
| Versión documentada | 1.0.0 |
| Estado del software | Funcional, con módulos pendientes |
| Estado mecánico | Prototipo pendiente de validación |
| Sistema principal | Ordenador HP |
| Controlador | Raspberry Pi 4 |
| Pantalla | MSI PRO MP161 E2U |
| Microcontroladores | Arduino Nano |
| Interfaz | React / TypeScript |
| Servicios | Python |
| Licencia | Apache-2.0 |

## 04. Arquitectura del terminal

Orbit Terminal utiliza dos plataformas informáticas con responsabilidades diferenciadas.

### Ordenador HP

El equipo HP actúa como plataforma informática principal.

Utiliza Windows 10 y proporciona los recursos del ordenador reutilizado.

Su integración permite acceder al escritorio y ejecutar las aplicaciones instaladas en el equipo.

### Raspberry Pi 4

La Raspberry Pi ejecuta los servicios de Orbit OS y gestiona la interfaz visible en la pantalla del terminal.

También proporciona conectividad con los microcontroladores y participa en la comunicación con el ordenador HP.

### Comunicación entre equipos

El ordenador HP y la Raspberry Pi se conectan mediante un enlace Ethernet directo.

Esta conexión permite intercambiar información y acceder a determinadas funciones del sistema principal.

La solución documentada utiliza:

- Sunshine en el HP.
- Moonlight en la Raspberry Pi.
- Servicios de comunicación desarrollados para Orbit OS.
- Autenticación mediante token para el protocolo de control.

La imagen del HP se transmite mediante streaming al entorno de la Raspberry Pi.

**La pantalla MSI está conectada a la Raspberry Pi, no directamente a ambos equipos.**

## 05. Hardware del proyecto

### Ordenador principal

El sistema utiliza un ordenador compacto HP desmontado para integrar sus componentes en la carcasa personalizada.

Entre los componentes contemplados se encuentran:

- Placa base mini-ITX.
- Procesador y sistema de refrigeración.
- Memoria RAM.
- Almacenamiento.
- Conectores de vídeo y comunicaciones.
- Fuente de alimentación externa.

La documentación mecánica identifica una placa de aproximadamente 170 × 170 mm y una altura máxima medida de 35 mm.

### Raspberry Pi 4

La Raspberry Pi actúa como plataforma de control.

Entre sus responsabilidades:

- Ejecución del entorno Orbit OS.
- Comunicación con el HP.
- Gestión de servicios.
- Lectura de controles físicos.
- Integración con componentes electrónicos.
- Presentación de la interfaz.

### Pantalla

| Característica | Especificación |
|---|---|
| Modelo | MSI PRO MP161 E2U |
| Tamaño | 15,6 pulgadas |
| Resolución | 1920 × 1080 |
| Tecnología de entrada | No táctil |
| Control | Ratón, teclado y controles físicos |

Aunque la pantalla instalada no es táctil, determinadas partes de la interfaz están preparadas para una interacción de este tipo.

### Almacenamiento

El diseño mecánico contempla la integración de un disco duro de 3,5 pulgadas.

El CAD utiliza parámetros basados en el estándar SFF-8301.

También se contempla una alternativa de 2,5 pulgadas mediante parámetros del modelo.

## 06. Electrónica y controles físicos

Orbit Terminal incorpora un sistema de controles destinado a proporcionar interacción física con el dispositivo.

### Arduino Nano de mandos

Un Arduino Nano basado en ATmega328P se utiliza para gestionar entradas físicas.

Entre los elementos contemplados:

- Potenciómetros.
- Pulsadores.
- Controles de selección.
- Acciones configuradas.
- Comunicación serie con la Raspberry Pi.

El sistema está preparado para interpretar las entradas recibidas desde el microcontrolador.

La documentación indica que el firmware está en uso, aunque los potenciómetros y pulsadores físicos aún no estaban conectados en el estado registrado.

### Arduino Nano de prácticas

El proyecto incorpora un segundo Arduino Nano dedicado a experimentación.

Este microcontrolador se plantea como una plataforma independiente de prácticas electrónicas.

La documentación contempla:

- Acceso a pines.
- Programación.
- Monitorización de entradas.
- Pantalla OLED.
- Integración con Ardu Lab.

### Pantalla OLED

El diseño contempla una pantalla OLED de 0,96 pulgadas asociada al sistema de prácticas.

El ejemplo de firmware está compilado, pero su funcionamiento sobre la placa física no figura como validado en el estado documentado.

### ESP8266

El diseño contempla un ESP8266 NodeMCU para funciones relacionadas con iluminación.

Se ha previsto su integración con WLED.

La identificación y conexión definitiva de la tira LED permanecen pendientes.

## 07. Orbit OS — Interfaz de usuario

La interfaz de Orbit OS está desarrollada mediante React y TypeScript.

Su objetivo es proporcionar un centro de control visual para los diferentes componentes del terminal.

### Diseño

La identidad visual se basa en:

- Fondo oscuro.
- Acentos ámbar.
- Paneles informativos.
- Indicadores de estado.
- Controles compactos.
- Navegación lateral.
- Información de telemetría.
- Presentación coherente entre secciones.

### Secciones principales

| Sección | Función |
|---|---|
| Inicio | Resumen general del terminal |
| Sistemas | Información del HP y la Raspberry Pi |
| Hardware | Estado de los componentes |
| Controles | Interacción con los mandos |
| Ardu Lab | Herramientas de electrónica |
| Herramientas | Utilidades del entorno |
| Configuración | Preferencias y ajustes |

### Modo de simulación

Orbit OS incorpora un modo de simulación para desarrollo y pruebas.

Cuando se utiliza, el sistema diferencia expresamente los datos simulados de los procedentes del hardware real.

La interfaz muestra el distintivo **MODO SIMULACIÓN**.

Los componentes físicos no conectados pueden aparecer deshabilitados para evitar presentar como operativas funciones todavía no disponibles.

## 08. Control y monitorización del HP

Orbit OS incorpora un agente destinado a ejecutarse en el ordenador HP.

Este componente permite intercambiar información con la Raspberry Pi y realizar determinadas acciones autorizadas.

### Telemetría

El agente proporciona información de:

- CPU.
- Memoria.
- Almacenamiento.
- Red.
- Temperatura, cuando está disponible.
- Estado del equipo.

### Acciones disponibles

Entre las operaciones documentadas se encuentran:

- Bloquear Windows.
- Ajustar el volumen.
- Silenciar el audio.
- Reproducir o pausar contenido.
- Reiniciar el sistema.
- Apagar el equipo.

Las operaciones de apagado y reinicio están sujetas a las condiciones de confirmación y seguridad implementadas.

### Seguridad

El sistema utiliza una lista blanca de acciones.

Esto significa que los comandos admitidos están definidos previamente, evitando interpretar cualquier mensaje recibido como una instrucción arbitraria del sistema operativo.

## 09. Visualización del escritorio HP

El proyecto utiliza Sunshine y Moonlight para acceder visualmente al sistema Windows desde la Raspberry Pi.

### Funcionamiento

Sunshine se ejecuta en el ordenador HP como servidor de streaming.

Moonlight funciona en la Raspberry Pi como cliente.

La imagen del escritorio Windows llega mediante la conexión Ethernet interna.

### Integración

El proyecto contempla dos modalidades visuales:

**Vista integrada**

El escritorio remoto se presenta dentro de la experiencia visual del terminal.

**Pantalla completa**

El streaming ocupa la pantalla cuando se selecciona este modo.

### Controles

El sistema documenta un mecanismo para cambiar el contenido visible mediante acciones del software y controles físicos.

Para la configuración completa, consultar:

[Instalación y configuración de Raspberry Pi](docs/instalacion-pi.md)

## 10. Ardu Lab

**Ardu Lab** es la sección orientada a la experimentación electrónica.

Su objetivo es ofrecer herramientas de interacción con los microcontroladores y componentes conectados al terminal.

### Funciones contempladas

- Gestión del Arduino de prácticas.
- Programación de microcontroladores.
- Consulta de entradas.
- Integración con dispositivos electrónicos.
- Desarrollo de proyectos experimentales.

La documentación contempla el uso de Arduino CLI para compilar y transferir firmware.

### Documentación

[Consultar Ardu Lab](docs/ardu-lab.md)

## 11. Diseño mecánico

Orbit Terminal utiliza una carcasa personalizada concebida para impresión 3D.

El diseño se desarrolla mediante OpenSCAD y se organiza en piezas imprimibles.

### Concepto

La carcasa adopta una geometría en cuña que permite integrar la pantalla, las placas y los elementos de control dentro de una estructura compacta.

### Componentes mecánicos

- Base.
- Carcasa.
- Bisel de pantalla.
- Soportes internos.
- Bandejas de componentes.
- Soporte de almacenamiento.
- Guías y elementos de fijación.
- Paneles de conectores.
- Piezas para controles.
- Elementos auxiliares.

### Dimensiones del CAD documentado

| Dimensión | Valor aproximado |
|---|---:|
| Anchura | 456,3 mm |
| Profundidad | 300,5 mm |
| Altura | 153,9 mm |

Estas dimensiones corresponden al diseño provisional documentado.

**No deben interpretarse como dimensiones certificadas de una carcasa final.**

### Impresión 3D

La documentación contempla:

- Material PLA+.
- Acabado negro mate.
- Preparación para Bambu Lab A1.
- División en 20 archivos STL.
- Comprobaciones de geometría y volumen de impresión.

Los modelos se consideran provisionales y deben validarse físicamente antes de fabricar el conjunto completo.

## 12. Documentación CAD y montaje

Orbit Terminal dispone de documentación técnica para continuar el desarrollo mecánico.

### Manual de montaje

El repositorio incluye un manual ilustrado de 21 páginas.

**[Consultar manual de montaje de Orbit Terminal](docs/manual-montaje/MANUAL_MONTAJE_ORBIT.pdf)**

El manual describe un procedimiento de ensamblaje del prototipo y contiene dibujos derivados del CAD.

No constituye una certificación de fabricación ni confirma que todos los componentes encajen físicamente.

### Estado de desarrollo

El documento principal de continuidad técnica es:

[Estado y traspaso del proyecto](docs/ESTADO-Y-TRASPASO.md)

Contiene referencias de hardware, medidas, elementos pendientes y procedimientos de verificación.

### Archivos de impresión

Los componentes y las siguientes etapas previstas de impresión se documentan en:

[Guía de impresión 3D](hardware/impresion/siguientes/README.md)

## 13. Arquitectura del software

Orbit OS utiliza distintos módulos especializados.

### Interfaz

**React + TypeScript + Vite**

Gestiona la presentación visual del entorno y la interacción con el usuario.

### orbitd

Servicio Python que actúa como componente central de comunicación de la Raspberry Pi.

Entre sus funciones:

- Servir la interfaz.
- Mantener comunicaciones WebSocket.
- Leer datos del Arduino.
- Interpretar controles.
- Coordinar mensajes.
- Gestionar los estados recibidos.

### hp-agent

Agente Python destinado al ordenador HP.

Proporciona telemetría y ejecuta las acciones autorizadas mediante el protocolo del proyecto.

### Protocolo compartido

El sistema incluye una especificación común para la comunicación entre servicios.

Contempla:

- Mensajes JSON.
- Autenticación mediante token.
- Comprobaciones de conexión.
- Definición de acciones.
- Esquemas de datos.
- Tipos compartidos.

**[Consultar protocolo de comunicación](software/shared/PROTOCOLO.md)**

### Firmware Arduino

El repositorio incluye el firmware de los controles y un ejemplo independiente para el Arduino de prácticas.

## 14. Tecnologías utilizadas

| Tecnología | Función |
|---|---|
| Python | Servicios y agentes |
| React | Interfaz de usuario |
| TypeScript | Desarrollo del frontend |
| Vite | Compilación de interfaz |
| WebSocket | Comunicación entre servicios |
| JSON | Protocolo y configuración |
| Arduino C/C++ | Firmware |
| OpenSCAD | Diseño CAD |
| Raspberry Pi | Plataforma de control |
| Windows 10 | Sistema del HP |
| Sunshine | Streaming desde Windows |
| Moonlight | Recepción del escritorio |
| Linux | Entorno de Raspberry Pi |
| GitHub Actions | Integración continua |
| pytest | Pruebas Python |
| Vitest | Pruebas del frontend |
| Ruff | Análisis estático |

## 15. Organización del repositorio

| Directorio o archivo | Contenido |
|---|---|
| `software/interface/` | Interfaz Orbit OS |
| `software/pi-controller/` | Servicio orbitd |
| `software/hp-agent/` | Agente Windows |
| `software/shared/` | Protocolo de comunicación |
| `software/arduino-controls/` | Firmware de mandos |
| `software/arduino-pruebas/` | Firmware de prácticas |
| `hardware/cad/` | Modelos OpenSCAD |
| `hardware/impresion/` | Archivos y herramientas de impresión |
| `hardware/render/` | Generación de renders |
| `assets/screenshots/` | Capturas de Orbit OS |
| `assets/renders/` | Visualizaciones CAD |
| `docs/` | Documentación técnica |
| `tests/python/` | Pruebas de servicios |
| `scripts/` | Automatización y desarrollo |
| `CHANGELOG.md` | Historial de cambios |
| `README.md` | Documentación principal |

## 16. Preparación del entorno de desarrollo

### Requisitos

- Python 3.9 o posterior.
- Node.js 20.
- npm.
- Git.
- Entorno compatible con los scripts utilizados.

Herramientas opcionales:

- Arduino CLI.
- Chrome o Chromium.
- OpenSCAD.
- Herramientas de impresión 3D.

### Clonar el repositorio

```bash id="tlp2gt"
git clone https://github.com/ardu01/Orbit-OS.git
cd Orbit-OS
```

### Preparar el entorno

```bash id="qgaf29"
./scripts/setup-dev.sh
```

Activar el entorno Python:

```bash id="53s4sn"
. .venv/bin/activate
```

### Ejecutar las pruebas

```bash id="a6h2oo"
./scripts/test-all.sh
```

### Iniciar la simulación

```bash id="6xsb74"
./scripts/dev-sim.sh
```

La interfaz simulada se sirve en:

`http://127.0.0.1:8765/`

### Ejecutar únicamente la interfaz

```bash id="9dn2nr"
cd software/interface
npm run dev
```

Dirección de desarrollo:

`http://localhost:5173`

## 17. Instalación en Raspberry Pi

La Raspberry Pi constituye el entorno principal de ejecución de Orbit OS.

### Preparación

El repositorio incluye un script de instalación destinado a preparar los servicios necesarios.

Antes de ejecutarlo es necesario revisar la documentación del hardware, la red y las dependencias.

### Generar token

```bash id="n4a81t"
./scripts/gen-token.sh
```

El token se almacena en un archivo `.env` excluido del control de versiones.

Debe mantenerse privado y compartirse con el HP únicamente mediante un canal seguro.

### Instalar en la Raspberry Pi

```bash id="1f9vbc"
sudo bash scripts/instalar-pi.sh
```

Después debe reiniciarse el sistema según las instrucciones de instalación.

### Documentación completa

[Guía de instalación en Raspberry Pi](docs/instalacion-pi.md)

Incluye la configuración del entorno, los servicios, el streaming y la salida del modo kiosco.

## 18. Configuración del HP

El ordenador HP utiliza un agente de software que proporciona telemetría y funciones de control.

La instalación requiere Windows 10 y la preparación correspondiente del entorno.

### Funciones del agente

- Enviar información del sistema.
- Mantener comunicación con Orbit OS.
- Ejecutar acciones autorizadas.
- Gestionar estados y respuestas.
- Aplicar mecanismos de seguridad.

### Instalación

El proyecto incluye:

`scripts/instalar-hp.ps1`

Para preparar la instalación, consultar:

[Guía de instalación del HP](docs/instalacion-hp.md)

El procedimiento requiere revisar el script antes de ejecutarlo con privilegios de administrador.

### Modo de prueba

La documentación contempla un modo `DryRun` que permite preparar el agente sin habilitar determinadas acciones de control.

Es recomendable utilizarlo durante las primeras comprobaciones.

## 19. Arduino y firmware

Orbit Terminal incorpora firmware específico para sus dos microcontroladores.

### Compilación

```bash id="p5c0pu"
./scripts/compile-arduino.sh
```

El script compila el firmware de controles y el ejemplo del Arduino de prácticas.

### Variantes

Se contempla compatibilidad con Arduino Nano ATmega328P y con clones que utilizan el bootloader antiguo.

Las opciones de compilación documentadas incluyen:

`arduino:avr:nano`

`arduino:avr:nano:cpu=atmega328old`

### Documentación específica

- [Arduino de controles](software/arduino-controls/README.md)
- [Arduino de prácticas](software/arduino-pruebas/README.md)

## 20. Estado de los componentes

La siguiente tabla resume el estado registrado en la documentación del proyecto.

| Componente | Estado |
|---|---|
| Interfaz Orbit OS 1.0.0 | En uso |
| Servicio orbitd | Implementado |
| Protocolo de comunicación v1 | Implementado |
| Agente del HP | En uso |
| Telemetría del HP | En uso |
| Streaming Sunshine / Moonlight | En uso |
| Servicios de Raspberry Pi | En uso |
| Firmware del Nano de mandos | En uso |
| Controles físicos cableados | Pendiente |
| Arduino de prácticas con OLED | Pendiente de validación |
| ESP8266 y WLED | Pendiente |
| Iluminación física | Pendiente de conexión |
| CAD mecánico | Provisional |
| Validación de la carcasa | Pendiente |
| Cifrado avanzado HP–Pi | Pendiente |

Los estados corresponden a la documentación del prototipo y no implican que todos los módulos estén preparados para distribución general.

## 21. Pruebas y validación

El proyecto incluye procedimientos automatizados para comprobar tanto el software como determinadas características del CAD.

### Pruebas documentadas

La ejecución registrada el 20 de octubre de 2026 incluyó:

| Comprobación | Resultado |
|---|---|
| Ruff | Sin avisos |
| pytest | 50 pruebas aprobadas |
| Vitest | 27 pruebas aprobadas |
| TypeScript | Compilación correcta |
| Vite | Compilación correcta |
| Arduino de controles | Compilación correcta |
| Arduino de prácticas | Compilación correcta |
| Verificación de interferencias | Sin interferencias detectadas |
| Verificación de STL | 20 mallas cerradas y dentro del volumen previsto |

### Consideraciones

Estas cifras corresponden a una ejecución histórica concreta.

No deben interpretarse como resultados de pruebas ejecutadas sobre cada modificación posterior.

El proyecto también registra pruebas prácticas del software en Raspberry Pi y HP.

### Validación física

La comprobación geométrica de un STL no garantiza que la pieza fabricada tenga tolerancias adecuadas.

Las verificaciones físicas de los componentes y del ensamblaje continúan siendo necesarias.

## 22. Seguridad

Orbit OS incorpora controles destinados a limitar las operaciones disponibles entre dispositivos.

### Autenticación

La comunicación de control utiliza un token generado para la instalación.

Los secretos locales deben permanecer fuera del repositorio.

### Lista blanca

Las acciones admitidas están definidas explícitamente.

No se proporciona ejecución arbitraria de comandos recibidos desde la red mediante el protocolo documentado.

### Conexión HP–Pi

La implementación documentada utiliza `ws://` con autenticación mediante token.

**Esta comunicación no incorpora cifrado de transporte en la versión descrita.**

Por tanto, debe utilizarse exclusivamente sobre un enlace directo o una red de confianza.

### Archivos sensibles

El proyecto excluye de Git archivos como:

- `.env`
- `*.token`
- `*.key`
- `*.pem`
- Configuraciones locales privadas.

### Precauciones de hardware

La documentación mecánica y eléctrica es experimental.

No deben fabricarse ni conectarse componentes sin revisar previamente las medidas, tensiones, protecciones y condiciones reales de montaje.

## 23. Limitaciones actuales

### Hardware

- Carcasa pendiente de validación física definitiva.
- Medidas pendientes de determinados componentes.
- Cableado incompleto de controles.
- Iluminación sin conexión definitiva.
- HAT VHF pendiente de caracterización mecánica completa.
- Validación pendiente del Arduino de prácticas con OLED.

### Software

- Módulos dependientes de hardware no conectado.
- Cifrado avanzado de transporte pendiente.
- Determinadas funciones disponibles únicamente en simulación.
- Dependencia de servicios externos para streaming.
- Necesidad de configurar individualmente HP y Raspberry Pi.

### Fabricación

Los STL y modelos mecánicos documentados no deben considerarse planos de producción final.

## 24. Hoja de ruta

### Fase I. Plataforma de software

- [x] Interfaz Orbit OS.
- [x] Protocolo de comunicación.
- [x] Servicio orbitd.
- [x] Agente HP.
- [x] Telemetría.
- [x] Integración Sunshine / Moonlight.
- [x] Simulación.
- [x] Pruebas automatizadas.

### Fase II. Electrónica

- [x] Firmware de controles.
- [x] Integración serie.
- [ ] Cableado definitivo de potenciómetros.
- [ ] Integración completa de pulsadores.
- [ ] Validación del Arduino de prácticas.
- [ ] Integración de iluminación.
- [ ] Comprobación del HAT VHF.

### Fase III. Hardware

- [x] Modelado CAD inicial.
- [x] División de piezas para impresión.
- [x] Generación de STL.
- [x] Comprobaciones geométricas iniciales.
- [ ] Validación dimensional de todas las piezas.
- [ ] Pruebas de ensamblaje.
- [ ] Ajustes de tolerancias.
- [ ] Validación mecánica completa.

### Fase IV. Consolidación

- [ ] Mejorar el cifrado de las comunicaciones.
- [ ] Completar la integración de controles.
- [ ] Ampliar la documentación de mantenimiento.
- [ ] Ejecutar una validación integral del terminal.
- [ ] Consolidar una versión de hardware reproducible.

Esta hoja de ruta representa posibles desarrollos y no establece fechas de entrega.

## 25. Documentación técnica

### Documentación general

- [Estado y traspaso](docs/ESTADO-Y-TRASPASO.md)
- [Historial de versiones](CHANGELOG.md)
- [Decisiones del prototipo](docs/decisiones-prototipo.md)

### Diseño mecánico

- [Diseño mecánico](docs/diseno-mecanico.md)
- [Manual de montaje](docs/manual-montaje/MANUAL_MONTAJE_ORBIT.pdf)
- [Planificación de impresión](hardware/impresion/siguientes/README.md)

### Electrónica

- [Controles](docs/controles.md)
- [Raspberry Pi](docs/raspberry-pi.md)
- [Ardu Lab](docs/ardu-lab.md)
- [Alimentación preliminar](docs/alimentacion-preliminar.md)

### Instalación

- [Instalación en Raspberry Pi](docs/instalacion-pi.md)
- [Instalación en HP](docs/instalacion-hp.md)

### Comunicación

- [Protocolo del sistema](software/shared/PROTOCOLO.md)
- [Firmware Arduino](software/arduino-controls/README.md)

## 26. Licencia y atribuciones

El proyecto se distribuye bajo **Apache License 2.0** conforme al archivo `LICENSE` del repositorio.

Los componentes de terceros utilizados en el sistema conservan sus propias licencias.

Entre ellos se encuentran:

- React.
- TypeScript.
- Vite.
- Python y sus dependencias.
- Arduino y herramientas relacionadas.
- Sunshine.
- Moonlight.
- OpenSCAD.
- Componentes de hardware y bibliotecas externas.

Los nombres y marcas de fabricantes se utilizan con fines descriptivos.

Orbit Terminal es un proyecto independiente y no implica afiliación o respaldo por parte de HP, MSI, Raspberry Pi u otros fabricantes.

## 27. Autor y organización

### Miguel Rodríguez Saiz

Diseño y desarrollo de Orbit Terminal y Orbit OS.

El proyecto reúne trabajo de diseño mecánico, electrónica, desarrollo de interfaces, integración de sistemas y experimentación tecnológica.

### Ardu Solutions

Iniciativa tecnológica dedicada al desarrollo de software, inteligencia artificial, electrónica, hardware y soluciones de ingeniería.

### Enlaces oficiales

**Web de Orbit Terminal**  
https://ardu01.github.io/orbit-web/

**Repositorio Orbit OS**  
https://github.com/ardu01/Orbit-OS

**Proyecto Control-deck**  
https://github.com/Sopa-IA/Control-deck

**Portfolio de proyectos**  
https://ardu01.github.io/proyectos/

**Ardu Solutions**  
https://ardusolutions.pages.dev/

**GitHub**  
https://github.com/ardu01

---

**© 2026 Miguel Rodríguez Saiz · Ardu Solutions**

**Orbit Terminal — Experimental Computing Platform**

*One terminal. Multiple systems. Endless possibilities.*
