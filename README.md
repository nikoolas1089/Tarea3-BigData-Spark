Tarea 3 - Procesamiento de Datos con Apache Spark
Descripción
Este proyecto corresponde a la Tarea 3 de Big Data y Analytics de la UNAD.

Se desarrollaron actividades de:

Procesamiento Batch utilizando Apache Spark.
Procesamiento en Tiempo Real utilizando Apache Kafka y Spark Streaming.
Análisis de un conjunto de datos de Netflix.
Implementación de un productor y consumidor de datos en tiempo real.
Dataset Utilizado
Netflix Titles Dataset

Archivo:

netflix_titles.csv
Tecnologías Utilizadas
Apache Spark 3.5.8
Apache Kafka 3.9.2
Python 3
PySpark
Ubuntu Linux
Resultados Obtenidos
Procesamiento Batch
Se realizaron las siguientes tareas:

Carga de datos.
Limpieza de datos.
Identificación de valores nulos.
Análisis de contenido por tipo.
Análisis por país.
Análisis por clasificación.
Análisis por año de lanzamiento.
Procesamiento en Tiempo Real
Se implementó:

Topic Kafka: sensor_data
Productor Kafka
Consumidor Spark Streaming
Los datos fueron procesados en tiempo real mediante Spark Streaming.

Ejecución
Iniciar ZooKeeper
sudo /opt/Kafka/bin/zookeeper-server-start.sh /opt/Kafka/config/zookeeper.properties
Iniciar Kafka
sudo /opt/Kafka/bin/kafka-server-start.sh /opt/Kafka/config/server.properties
Ejecutar Productor
python3 kafka_producer.py
Ejecutar Consumidor
/opt/spark/bin/spark-submit \
--packages org.apache.spark:spark-sql-kafka-0-10_2.12:3.5.3 \
spark_streaming_consumer.py
Autor
Nicolás Cuartas Martínez

Universidad Nacional Abierta y a Distancia - UNAD

Ejecución del Proyecto
Procesamiento Batch
Iniciar PySpark:

/opt/spark/bin/pyspark

Ejecución del Proyecto
Procesamiento Batch
Iniciar PySpark:

/opt/spark/bin/pyspark
sudo /opt/Kafka/bin/zookeeper-server-start.sh /opt/Kafka/config/zookeeper.properties
sudo /opt/Kafka/bin/kafka-server-start.sh /opt/Kafka/config/server.properties
python3 kafka_producer.py
/opt/spark/bin/spark-submit \
--packages org.apache.spark:spark-sql-kafka-0-10_2.12:3.5.3 \
spark_streaming_consumer.py
---

### Agregar después de "Resultados Obtenidos"

```markdown
## Conclusiones

- Apache Spark permitió procesar eficientemente el dataset de Netflix.
- Se analizaron 8.809 registros de películas y series.
- Estados Unidos e India presentaron la mayor cantidad de contenido.
- El procesamiento batch permitió obtener información descriptiva del conjunto de datos.
- Kafka y Spark Streaming facilitaron el procesamiento de datos en tiempo real.
