# De que imagen se basa
FROM ubuntu

# Dependencias del sistema
RUN apt update -y
RUN apt-get install -y python
RUN apt-get install -y python3-pip

# Dependencias de python
RUN pip install flask

# Copiar archivos a la imagen
COPY app.py /opt/

# Run the application
ENTRYPOINT FLASK_APP=/opt/app.py flask run --host=0.0.0.0 --port=8080