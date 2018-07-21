FROM ubuntu

COPY requirements.txt /requirements.txt

# Install general dev tools
RUN apt-get update && \
    apt-get install -y tzdata && \
    apt-get install -y \
    wget \
    python2.7 \
    python-pip \
    python-dev \
    ipython \
    jupyter \
  && rm -rf /var/lib/apt/lists/*

# Install python requirements
RUN pip install --upgrade pip
RUN pip install -r requirements.txt

# Make workspace
RUN mkdir /workspace

EXPOSE 8888

# Launch Jupyter notebook
CMD ["jupyter-notebook","--allow-root", "--ip=0.0.0.0", "--notebook-dir=/workspace"]
