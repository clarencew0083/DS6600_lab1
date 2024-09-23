# syntax=docker/dockerfile:1

FROM python:3.11.4-bookworm

# Copy the requirements.txt file into the container
COPY requirements.txt requirements.txt

# Install packages from requirements.txt using pip
RUN pip install --upgrade pip && pip install -r requirements.txt

WORKDIR /problem5

EXPOSE 8888

CMD ["jupyter", "lab","--ip=0.0.0.0","--allow-root"]