FROM python:3.10-slim-buster

# Inside container
# Make a new folder inside container
WORKDIR /backend-flask

# Outside container -> Inside container
# This contains the libraries we want to install to run the app
COPY requirements.txt requirements.txt

# Inside container
# Install the python libraries used for the application
RUN pip3 install -r requirements.txt

# Outside container -> Inside container
# . means everything in the current directory
# First . represents everything in /backend-flask (outside container)
# Second . represents everything in /backend-flask (inside container)
COPY . .

# Set Environment Variables (Env Vars)
# Inside container and will remain set when container is running
ENV FLASK_ENV=development

EXPOSE ${PORT}

# CMD (Command)
# python3 -m flask run --host=0.0.0.0 --port=4567
CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=4567"]