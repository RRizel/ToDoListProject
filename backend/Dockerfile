FROM python:3

WORKDIR /usr/sec/app

# Copy the requirements file and install dependencies
COPY requirements.txt ./
RUN pip install --no-cache-dir --upgrade -r requirements.txt

# Copy the rest of the backend application code (src folder)
COPY ./src /usr/sec/app/src

EXPOSE 3001

# Command to run the server
CMD [ "python", "./src/server.py"]
