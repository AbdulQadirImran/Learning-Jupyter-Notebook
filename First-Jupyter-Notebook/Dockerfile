# Use an official Python runtime as a parent image
FROM python:3.12

# Set the working directory in the container
WORKDIR /usr/src/app

# Install Jupyter
RUN pip install notebook

# Copy the current directory contents into the container at /usr/src/app
COPY . .

# Expose port 8888 to the outside world
EXPOSE 8888

# Command to run Jupyter Notebook
CMD ["jupyter", "notebook", "--ip=0.0.0.0", "--port=8888", "--no-browser", "--allow-root"]