FROM python:3.13

ENV VIRTUAL_ENV=/opt/venv
RUN python3 -m venv $VIRTUAL_ENV

#NB: PATH="$VIRTUAL_ENV/bin:$PATH" may be indirectly done via /opt/venv/bin/activate && ... 
ENV PATH="$VIRTUAL_ENV/bin:$PATH"

# Install required Python packages in the virtual environment.
RUN pip install pytest

# Install application specific dependencies:
#COPY requirements.txt .
#RUN pip install -r requirements.txt

# Run the application:
#COPY myapp.py .
#CMD ["python", "myapp.py"]
