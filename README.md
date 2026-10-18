# Visor & Dashboard Proyecto Solar Fotovoltaico vr 1.0

Visor geográfico interactivo de alta precisión para el seguimiento integral de obras de energía solar fotovoltaica utility-scale (200 MWp / 160 MW AC): avance físico de bloques solares, subestación elevadora, línea de transmisión, cumplimiento ambiental y relacionamiento comunitario.

---

## ☀️ Resumen Técnico del Proyecto

- **Nombre:** Parque Solar Fotovoltaico Sol de La Guajira 200 MWp
- **Ubicación:** Departamento de La Guajira, Colombia
- **Potencia Pico (DC):** 196.8 MWp
- **Potencia Nominal (AC):** 160.0 MW AC
- **Superficie Ocupada:** 324.5 hectáreas
- **Tecnología de Módulos:** Módulos bifaciales monocristalinos N-Type TOPCon de 600Wp (328.000 paneles)
- **Estructura de Soporte:** Seguidores solares a un eje monofila (1P Trackers con backtracking anti-sombras)
- **Centros de Transformación:** 10 Skids de 3.5 MVA (Inversor centralizado + transformador 0.69/34.5 kV)
- **Subestación Elevadora:** SE Guajira Solar 34.5 / 110 kV con transformador de potencia de 160 MVA y sistema de baterías BESS (20 MW / 40 MWh)
- **Línea de Evacuación:** LAT 110 kV de 8.75 km con 18 torres metálicas de celosía
- **Generación Limpia Estimada:** 415 GWh / año (Equivalente al consumo de 210.000 hogares)
- **Emisiones Mitigadas:** 186.750 Toneladas de CO₂eq / año

---

## 📌 Módulos del Tablero de Control

1. **📋 Programación Semanal de Obra:**
   - Visualización de frentes de trabajo por día (Lunes a Viernes y Resumen Semanal).
   - Filtrado y resaltado reactivo en el mapa: ilumina los bloques fotovoltaicos, torres de la línea o puntos ambientales programados para cada jornada.
   - Actividades especializadas: hincado mecánico con guía láser, montaje de trackers, instalación de módulos bifaciales, zanjeo y tendido de cableado DC string, pruebas I-V y comisionamiento.

2. **☀️ Avance Bloques Solares (EPC):**
   - Tarjetas KPI estilo ArcGIS Online con semáforos porcentuales:
     - *Hincado de Pilotes*
     - *Montaje de Estructura / Trackers*
     - *Instalación de Módulos Solares*
     - *Zanjeo y Canalizaciones BT/MT*
     - *Cableado de Strings DC*
     - *Comisionamiento y Pruebas Eléctricas*
   - Comportamiento reactivo: Al hacer clic en cualquier Bloque FV en el mapa o en el selector desplegable, expone el progreso individual del bloque seleccionado; al pulsar "↺ Ver Todo", recalcula el promedio ponderado consolidado del parque.

3. **⚡ Subestación & Línea de Evacuación (LAT 110 kV):**
   - Monitoreo del avance de obra civil y montaje electromecánico de la Subestación Elevadora Guajira Solar 34.5/110 kV, celdas GIS y sistema BESS.
   - Inspección estructura por estructura (ST-01 a ST-18) de la línea de alta tensión: excavación, cimentación, izaje y tendido de conductores y cable de guarda OPGW.

4. **🌿 Gestión Ambiental & Biótica:**
   - Cumplimiento de compromisos del Plan de Manejo Ambiental (PMA) y licencia ANLA.
   - Monitoreo de fauna: conteo de especímenes ahuyentados, rescatados y reubicados en corredores biológicos.
   - Rescate de flora y veda: aclimatación de cactáceas y epífitas en el vivero temporal *in situ*.
   - Obras de drenaje pluvial: seguimiento a alcantarillas de alivio, disipadores de energía y trampas de sedimentos.
   - Compensación forestal (1% Ley 99): restauración ecológica con especies nativas del bosque seco tropical.

5. **👥 Entorno Social & Comunidades:**
   - Conteo territorial y semáforo de relacionamiento social (122 comunidades):
     - 🟢 *Verde:* Diálogo fluido, convenios vigentes y acuerdos protocolizados.
     - 🟡 *Amarillo:* En mesas de concertación y atención a compromisos.
     - 🔴 *Rojo:* Alerta prioritaria / Diálogo urgente requerido.
   - **Filtro Espacial Interactivo:** Al pulsar cualquiera de las tarjetas de semáforo, el mapa enfoca automáticamente el área de ese grupo y atenúa las demás.
   - Ficha técnica comunitaria: distancia al parque solar, mano de obra local contratada, proyecto social fotovoltaico asignado y bitácora de reuniones.

---

## 📂 Capas Geoespaciales Abiertas (GeoJSON WGS 84)

| Capa | Archivo GeoJSON | Tipo | Descripción |
| :--- | :--- | :--- | :--- |
| **Bloques Solares** | `geojson/Bloques_Solares.geojson` | `Polygon` (10) | Polígonos de los 10 subcampos solares con avances físicos |
| **Área del Parque** | `geojson/Area_Parque_Solar.geojson` | `Polygon` (1) | Polígono perimetral con cerramiento de seguridad |
| **Inversores / Skids** | `geojson/Inversores_Transformadores.geojson` | `Point` (10) | Centros de transformación e inversión centralizada |
| **Subestación Solar** | `geojson/Subestacion_Solar.geojson` | `Polygon` / `Point` | Subestación Elevadora 34.5 / 110 kV y patio de llaves |
| **Línea Transmisión** | `geojson/Linea_Transmision.geojson` | `LineString` / `Point` (18) | Trazado LAT 110 kV y estructuras metálicas de celosía |
| **Estación Solar** | `geojson/Estacion_Meteorologica.geojson` | `Point` (1) | Estación meteorológica con piranómetros Clase A |
| **Gestión Ambiental** | `geojson/Obras_Drenaje_Ambientales.geojson` | `Point` (9) | Obras de drenaje, vivero, pasos de fauna y compensación |
| **Comunidades** | `geojson/Comunidades.geojson` | `Point` (122) | Asentamientos del área de influencia con atributos sociales |
| **Municipios** | `geojson/Municipios.geojson` | `MultiPolygon` | Límites territoriales municipales de referencia |

---

## 💻 Ejecución Local en el Portátil

El visor funciona al 100% de manera estática en el navegador sin requerir bases de datos externas ni Node.js pesado.

Para ejecutarlo localmente:

1. Abrir una terminal en la carpeta del proyecto:
   ```bash
   cd /Users/efrainlav/Downloads/Dashboard-Proyecto-Fotovoltaico
   ```

2. Iniciar el servidor local HTTP (requerido para permitir peticiones `fetch` de GeoJSON locales):
   ```bash
   # Opción recomendada con Python:
   python3 -m http.server 8000
   ```

3. Abrir en el navegador:
   ```text
   http://localhost:8000
   ```

---

## ⚠️ Declaración de Datos de Seguimiento (Datos Demo)

Los datos de avance físico, cronogramas y registros de bitácora han sido generados con fines ilustrativos, didácticos y de prototipado técnico de tableros de control GIS para la industria de energía renovable no convencional.
