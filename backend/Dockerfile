# Use Python 3.8
FROM python:3.8

# Set working directory
WORKDIR /app

# Install Poetry
RUN pip install poetry

# Set Poetry config to install packages system-wide
RUN poetry config virtualenvs.create false

# Copy only requirements to cache them in docker layer
COPY pyproject.toml ./

# Generate lock file and install dependencies
RUN poetry lock && poetry install

# Copy all files
COPY . /app

# Run FastAPI
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8080"]