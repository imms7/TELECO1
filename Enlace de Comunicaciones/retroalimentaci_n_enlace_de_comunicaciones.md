# 📡 Evaluación: Enlace de Comunicaciones

**Nota:** `4.6 / 5.0` *(15%)*

---

## 💬 Retroalimentación General

Felicitaciones por el trabajo desarrollado. El proyecto evidencia dedicación, investigación y una buena aplicación de los fundamentos de diseño de radioenlaces digitales. Se destaca que, después de evaluar la inviabilidad del enlace directo entre la **Universidad del Quindío** y la **Universidad del Tolima**, proponen una arquitectura de **seis radioenlaces y cinco estaciones repetidoras activas** para superar las dificultades topográficas de la Cordillera Central.

---

## 📊 Análisis de Resultados (Radio Mobile)

Los resultados muestran condiciones favorables a lo largo de la arquitectura propuesta:

* **Universidad del Quindío – Buenavista:** $10,2\text{ km}$, $-43,0\text{ dBm}$ y despeje de $7,6\text{ }F_1$.
* **Buenavista – La Línea:** $5,0\text{ km}$, $-42,0\text{ dBm}$ y despeje de $19,4\text{ }F_1$.
* **La Línea – Cajamarca:** $5,3\text{ km}$, $-45,9\text{ dBm}$ y despeje de $3,2\text{ }F_1$.
* **Cajamarca – Coello *(Tramo crítico)*:** $16,3\text{ km}$, constituye correctamente el enlace más exigente de la arquitectura, con una potencia recibida de $-55,9\text{ dBm}$, pérdidas de propagación de $142,1\text{ dB}$ y un despeje de $2,0\text{ }F_1$.
* **Coello – Martinica:** $11,3\text{ km}$, $-52,4\text{ dBm}$ y despeje de $10,9\text{ }F_1$.
* **Martinica – Universidad del Tolima:** $5,0\text{ km}$, $-41,6\text{ dBm}$ y despeje de $5,5\text{ }F_1$.

---

## ⚙️ Parámetros Técnicos y Ajustes Requeridos

Es positivo que incorporen la modulación, el ancho de canal y la sensibilidad del receptor como elementos de diseño para verificar la capacidad de transportar el video Full HD de $8\text{ Mbps}$. Sin embargo, se requieren los siguientes ajustes técnicos:

1. **Corrección según Datasheet (AF-5XHD):** Para $64\text{QAM}$ MIMO y $10\text{ MHz}$, la sensibilidad oficial es de **$-78\text{ dBm}$**, y la capacidad nominal agregada corresponde a **$69,12\text{ Mbps}$** ($34,56\text{ Mbps}$ por sentido con TDD simétrico). Con esta sensibilidad, el tramo crítico Cajamarca–Coello tendría un margen de **$22,1\text{ dB}$**, suficiente como resultado preliminar.
2. **Distribución TDD y Modulación:** Justificar la capacidad estimada para la distribución TDD $75/25$ y analizar cómo una reducción de la modulación podría afectar la continuidad del video.
3. **Documentación y Regulación:** Completar las coordenadas y elevaciones de los cinco repetidores, verificar los patrones de radiación de las antenas y comprobar el cumplimiento de las restricciones regulatorias de potencia, especialmente en los tramos con mayores niveles de recepción.

> *Estos ajustes son fundamentales para que la solución no solamente presente resultados favorables en simulación, sino que esté sustentada mediante parámetros técnicos verificables y condiciones reales de implementación.*

---

## 🎥 Video de Sustentación

Se destaca la participación de ambos estudiantes, quienes explican adecuadamente las razones técnicas y geográficas que justifican la utilización de varios saltos de radioenlace en lugar de una conexión directa entre las universidades. Asimismo, se evidencia un buen manejo de los parámetros configurados en Radio Mobile y capacidad para relacionar las características del terreno, las pérdidas de propagación, las alturas de las antenas y los resultados de recepción con las decisiones de diseño. La sustentación complementa el informe y demuestra comprensión del proceso seguido para construir la solución.

* **Recomendación:** Profundizar en la relación entre la potencia recibida, la sensibilidad del receptor, la modulación seleccionada y la velocidad efectiva de transmisión, explicando por qué el tramo más desfavorable determina el desempeño extremo a extremo de la red. Considerar también que la continuidad del servicio depende de la disponibilidad de cada repetidor, la interferencia, la alimentación eléctrica y las condiciones reales de operación.

---

## 🌍 Viabilidad Física, Ambiental y Regulatoria

En un proyecto de implementación real, la selección de los emplazamientos para las estaciones repetidoras no puede fundamentarse exclusivamente en los resultados favorables de Radio Mobile. Para los cinco repetidores propuestos (**Buenavista, La Línea, Cajamarca, Coello y Martinica**), es necesario realizar una evaluación preliminar antes de considerar técnicamente viable su implementación:

* **Infraestructura y Acceso:** Condiciones de acceso al terreno, disponibilidad para instalar torres o soportes, suministro de energía eléctrica y posibilidades de mantenimiento.
* **Entorno:** Condiciones climáticas y exposición a fenómenos naturales.
* **Normatividad:** Identificación de restricciones ambientales, áreas protegidas, condiciones de uso del suelo y permisos requeridos para la instalación de infraestructura de telecomunicaciones.