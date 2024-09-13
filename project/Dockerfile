FROM python:3.12-slim

# Create a directory for the project
RUN mkdir /project

# Set the working directory to /project
WORKDIR /project

# Copy the current directory contents into the container at /project
COPY . /project

# Install pip packages from requirements.txt
COPY requirements.txt /project/
RUN pip install -r requirements.txt

# Install Jupyter Notebook
RUN pip install jupyter

# Expose port 8888 for Jupyter Notebook
EXPOSE 8888

# Command to run Jupyter Notebook
CMD [ "jupyter", "notebook", "--ip=0.0.0.0", "--allow-root", "--no-browser" ]
