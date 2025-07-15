# logistica_empresa
# 📦 Simulación: Análisis de Inventario y Logística

Este proyecto simula el trabajo de un Logistics Analyst II, analizando discrepancias entre el inventario físico y registrado, consumo diario y alertas de bajo stock para 5 componentes clave: Motor, Circuito, Sensor, Batería y Panel.

---

## 🧠 Objetivo
Detectar errores operativos, evitar paros por falta de material y proponer mejoras al sistema de inventario.

---

## 📌 Acciones realizadas

- Cálculo de diferencia diaria entre inventario físico y registrado.
- Análisis del consumo total y promedio diario por componente.
- Identificación de fechas con alertas de bajo stock.
- Visualización con gráficos de línea por componente.

---

## 📈 Resultados clave

| Indicador                              | Valor         |
|----------------------------------------|---------------|
| Componente con mayor discrepancia      | Motor (14 u.) |
| Discrepancia promedio total            | 2.0           |
| Total de alertas de bajo stock         | 5             |
| Componente más consumido               | Batería (30 u.) |
| Consumo promedio diario                | 3.8           |

🔍 1. Discrepancia Promedio de Inventario: 2.0 unidades
📌 Interpretación:
Esto indica que en promedio, hay una diferencia de 2 unidades entre el inventario registrado y el físico por día por componente.

✅ Mejoras recomendadas:

Auditorías semanales para componentes con discrepancia >2.
Implementar un proceso doble de validación al registrar entradas/salidas.
Automatizar alertas si la discrepancia supera el 5% del stock registrado.
Introducir códigos de escaneo o tablets para registrar salidas en tiempo real.
🔍 2. Total de Alertas de Bajo Stock: 5 alertas (concentradas en Sensor)
📌 Interpretación:
Se presentaron 5 momentos críticos donde el inventario físico cayó por debajo del mínimo esperado.

✅ Mejoras recomendadas:

Revisar el punto de reorden (reorder point) del componente Sensor.
Establecer inventario mínimo dinámico en función del consumo y lead time.
Crear un sistema de alerta automática en dashboard si quedan menos de 3 días de stock (usando consumo promedio).
Incluir al equipo de compras en el flujo de notificaciones preventivas.
🔍 3. Consumo Promedio Diario: 3.8 unidades
📌 Interpretación:
En promedio, se consumen casi 4 unidades por componente al día, aunque algunos como Batería alcanzan 5.

✅ Mejoras recomendadas:

Utilizar este valor para calcular el inventario de seguridad.
Ajustar frecuencia de reabastecimiento (por ejemplo, cada 5 días) para evitar exceso o falta de inventario.
Incorporar esta métrica en un sistema de planificación de demanda simple.
💡 Extra: Discrepancia total por componente
Componente	Discrepancia Total
Motor	14
Sensor	13
✅ Mejoras recomendadas:

Motor y Sensor deben priorizarse en el programa de control físico.
Evaluar si hay errores humanos recurrentes con estos componentes (como registros manuales mal hechos).
---

## 🛠️ Tecnologías usadas
- Python (pandas, matplotlib, seaborn)
- Tableau (opcional)
- Jupyter Notebook
- GitHub

---

## 📂 Estructura
- `/data`: CSV simulado con 30 días de inventario
- `/notebooks`: Análisis completo paso a paso
- `/img`: Visualizaciones de inventario

---

## 👤 Autor
José Ángel Mercado Vázquez  
[LinkedIn](https://www.linkedin.com/in/jose-angel-mercado-vazquez) | [GitHub](https://github.com/Angelitomixmatalosjaja)
