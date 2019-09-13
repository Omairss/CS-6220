RUN  /bin/bash -c "/opt/conda/bin/conda install jupyter -y --quiet \
	&& mkdir /opt/notebooks"
RUN pip install pandas-datareader \
	&& pip install tensorflow \
	&& pip install keras \
	&& pip install matplotlib \
	&& pip install numpy \
	&& pip install sklearn \
	&& pip install mnist \
	&& pip install tqdm\
	&& apt-get install htop


CMD /opt/conda/bin/jupyter notebook --notebook-dir=/opt/notebooks \
	--ip='*' --port=8888 --no-browser --allow-root
