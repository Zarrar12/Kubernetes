FROM ubuntu:20.04

RUN apt-get update && \
	DEBIAN_FRONTEND=noninteractive apt-get install -y python3 \
	python3-pip \
	cmake
	
RUN	pip3 install flask \
	scikit-build

COPY . /gzl_proj
WORKDIR /gzl_proj
RUN pip install -r requirements.txt
CMD ["python3", "app.py"]