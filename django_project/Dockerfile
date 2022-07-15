FROM python:3.8   
ENV DockerHOME=/django_project  
RUN mkdir -p $DockerHOME  
WORKDIR $DockerHOME  
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1  
RUN pip install --upgrade pip  
COPY . $DockerHOME  
RUN pip install -r requirements.txt  
EXPOSE 3000
CMD [ "python", "manage.py","runserver", "0.0.0.0:3000" ]