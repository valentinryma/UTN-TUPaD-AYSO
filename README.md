# Trabajo Práctico – Escaneo de Puertos con Nmap


## Integrantes
- **Rolando Nebrada – Comisión 9**
*Encargado de la presentación teórica.*


- **Valentín Rymasewski – Comisión 3**
*Encargado del ejercicio práctico y demostración técnica.*

---


## Video Explicativo del Trabajo
➡️ **[Video de explicación completa del trabajo práctico](https://drive.google.com/file/d/1lc76_hNT8kepvCliFCpLHme7-biLxvFc/view?usp=sharing)**




---


## Descripción del Proyecto
Este trabajo práctico tiene como objetivo analizar conceptos fundamentales de **ciberseguridad**, específicamente relacionados con técnicas de reconocimiento mediante **escaneo de puertos**.


A través de diferentes pruebas realizadas con **Nmap**, se busca identificar puertos abiertos, servicios en ejecución y potenciales superficies de ataque. Además, se incluye la simulación de un puerto expuesto y la posterior demostración de cómo cerrarlo de manera segura.


---


## Contenidos del Trabajo
- **Comandos utilizados** durante el escaneo de puertos.
- **Resultados obtenidos** con diferentes parámetros de Nmap.
- **Demostración práctica** de:
- Exponer un puerto manualmente usando una herramienta de escucha.
- Detectar dicho puerto con Nmap.
- Finalizar el proceso asociado para cerrar el puerto.
- **Conclusiones** sobre la importancia de minimizar la cantidad de puertos abiertos.


---


## Herramientas Utilizadas
- **Nmap**: análisis de puertos y servicios.
- **Netcat / Ncat** (según entorno): apertura de puertos para pruebas.
- **Windows / Linux** (dependiendo del sistema usado en la práctica).

## Ejecución de las Pruebas


### 1. Escaneo inicial de puertos
```bash
nmap -sS <IP_OBJETIVO>
```


### 2. Escaneo con parámetros adicionales
```bash
nmap -sV -O <IP_OBJETIVO>
```


### 3. Apertura de un puerto en escucha
```bash
nc -l -p 12345 -v
```


### 4. Verificación del puerto abierto
```bash
nmap -sS <IP_OBJETIVO>
```


### 5. Cierre del puerto
- Identificación del proceso asociado.
- Finalización del proceso (kill / taskkill según SO).


---

## Resultados
Los resultados muestran:
- Detección correcta del puerto previamente expuesto.
- Variación de puertos identificados según el tipo de escaneo.
- Confirmación de la importancia de cerrar puertos no utilizados para minimizar la superficie de ataque.


---


## Conclusiones
Mantener solo los puertos estrictamente necesarios reduce significativamente el riesgo de accesos no autorizados. El uso de herramientas como Nmap permite auditar el estado real de la red y detectar configuraciones inseguras.

---

## Autoría
Trabajo realizado en el marco de la **materia [Nombre de la materia]** – Año [2025].
