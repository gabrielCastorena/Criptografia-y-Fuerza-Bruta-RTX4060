# Benchmarks RTX 4060 hashcat

Se corrieron benchmarks generales utilizando **hashcat** en una **rtx 4060**, solo por motivos de analisis generales de rendimiento.

### Especificaciones del sistema

* **GPU:** NVIDIA GeForce RTX 4060 (8GB VRAM)
* **CPU:** AMD Ryzen 5 5600G with Radeon Graphics
* **OS:** Windows
* **RAM:** 16 GB
* **Herramienta:** Hashcat v7.1.2
* **Runtime:** OpenCL 3.0 CUDA 13.1

### Configuracion del Proyecto

Configure el repositorio actual de GitHub para documentar los resultados, aunque tambien tuve que agregar un **.gitignore** para no subir diccionarios pesados como lo fue el **rockyou.txt** que se encuentra cargado en la misma carpeta.

Instale el respectivo **hashcat** y en la terminal ejecute el siguiente comando para correr los benchmarks y pasar todos los resultados automaticamente a un archivo de texto:

`hashcat.exe -b > benchmark_completo.txt`


### Resultados de Velocidad

| Algoritmo | Modo | Velocidad (Velocidad de Cracking) |
| :--- | :--- | :--- |
| **MD5** | 0 | 29.2 GH/s |
| **SHA2-256** | 1400 | 3.9 GH/s |
| **NTLM** | 1000 | 51.1 GH/s |

### Conclusion

Gracias a estos benchmarks logre aprender de manera sencilla la diferencia de velocidades entre hash simple y complejos junto con la potencia de mi grafica.