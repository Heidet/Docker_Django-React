# Pull base image
FROM python:3.9
# Set environment variables
ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1
# Set work directory
WORKDIR /opt
# Install dependencies
COPY ./requirements.txt /opt/
RUN pip install -r requirements.txt
# Copy project
COPY . /opt/
EXPOSE 8010
