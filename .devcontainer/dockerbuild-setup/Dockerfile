# we use the image with base python 3.11 and install requirements.txt on top this image
FROM python:3.11-bookworm

#copy the requirements.txt to image temp folder
COPY requirements.txt /tmp/requirements.txt

#run the installation
RUN pip3  --no-cache-dir install -r /tmp/requirements.txt \
    && rm -rf /tmp/requirements.txt

    #we can remove the temp file in the image to save space
    # we can now go to the devcontainer.json file and build the dev container
    #from this dockerfile
