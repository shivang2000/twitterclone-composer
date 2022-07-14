FROM python:3.8.10-buster

# setting working directory to backend
WORKDIR backend



# copy entrypoint.sh and set it to executable 
COPY docker-compose/backend/entrypoint.sh /
RUN chmod +x /entrypoint.sh

# RUN useradd -ms /bin/bash backend
# USER backend

# upgrading pip 
RUN pip install pip --upgrade   

# copy and install requirements.txt
COPY ./backend/requirements.txt requirements.txt
RUN pip install -r requirements.txt


EXPOSE 8000


ENTRYPOINT [ "/entrypoint.sh" ]