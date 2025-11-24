# 🔐 Verificador de Seguridad de Contraseñas

## Descripción general
Este proyecto es un script en Python que simula distintos métodos de verificación y análisis de contraseñas.  
Permite evaluar la seguridad de una contraseña según su longitud, conjunto de caracteres, entropía y número estimado de combinaciones necesarias para descubrirla.

El usuario puede elegir entre:
- Un método **exhaustivo ordenado** (fuerza bruta sistemática).
- Un método **inteligente** (descubre la contraseña carácter por carácter).
- Un **análisis detallado** que calcula entropía, combinaciones y clasificación de seguridad.

> **Nota educativa:** Este proyecto existe únicamente para fines didácticos.  
> No debe usarse para intentar vulnerar sistemas reales.

---

## Características principales
- **Validación de caracteres** (incluye letras con “Ñ”, números y símbolos comunes).
- **Análisis de entropía** según el tamaño real del conjunto usado.
- **Estimación de tiempo de crackeo** basada en ~1,000,000 intentos/segundo.
- **Modo exhaustivo ordenado:** prueba todas las combinaciones desde longitud 1 hasta la longitud de la contraseña.
- **Modo inteligente:** encuentra cada carácter mediante iteración secuencial.
- **Análisis detallado:** entropía, combinaciones, clasificación y tiempos estimados.
- **Protección ante overflow matemático** para contraseñas muy largas.

---

## Requisitos
- Python 3.x  
- No requiere bibliotecas externas  
- Módulos estándar usados: `random`, `math`, `time`, `itertools`

---

## Instalación
```bash
git clone https://github.com/JosueXT/Password-Security-Checker.git
cd Password-Security-Checker
python Password-Security-Checker.py
```
## Uso
1. Ejecuta:
 ```python Password-Security-Checker.py```
2. Ingresa la contraseña que deseas analizar.

Selecciona uno de los modos:

1 → Verificación exhaustiva ordenada

2 → Verificación inteligente

3 → Análisis detallado de seguridad

Observa en pantalla el progreso y el análisis final.
  
## Contribuciones
¡Las contribuciones son bienvenidas! Si quieres mejorar el código (ej. agregar más caracteres, optimizar cálculos o traducir a otros idiomas), sigue estos pasos:
1. Haz un fork del repositorio.
2. Crea una rama para tu feature: `git checkout -b feature/nueva-funcion`.
3. Haz commit de tus cambios: `git commit -m "Agrega nueva función"`.
4. Push a la rama: `git push origin feature/nueva-funcion`.
5. Abre un Pull Request.

## Licencia
Este proyecto está bajo la Licencia MIT. Consulta el archivo `LICENSE` para más detalles.

## Disclaimer (Liberación de Responsabilidad)
Este proyecto ha sido desarrollado únicamente con fines éticos y educativos, para demostrar conceptos de seguridad informática y criptografía. El autor no se hace responsable de cualquier uso indebido, ilegal o no ético de esta herramienta. No se debe utilizar para intentar crackear, acceder o comprometer contraseñas reales de terceros, ya que esto viola leyes de privacidad, protección de datos y ética digital. El usuario asume toda la responsabilidad por el uso que le dé a este código. Recuerda: en la práctica, las contraseñas se protegen con hashing y salting, haciendo el cracking real inviable.

## Notas de seguridad

Uso exclusivo con fines educativos.

No debe utilizarse para vulnerar contraseñas reales.

El uso indebido puede ser ilegal y antiético.
## Créditos
- Desarrollado por @JosueXT como proyecto educativo.
- Inspirado en conceptos de criptografía y seguridad informática.
- Agradecimientos a la comunidad de Python por los módulos estándar.

## Contacto
Si tienes preguntas o sugerencias, abre un issue en GitHub.

¡Gracias por usar este proyecto! Recuerda: 
La mejor seguridad es usar contraseñas únicas y gestores de contraseñas. 🔒
