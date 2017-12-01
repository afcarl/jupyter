# jupyter

Jupyter environment and examples in 

Build docker

	docker build -t knockdata/jupyter .

Run the Docker

	docker run -it --rm -p 8888:8888 -v `pwd`:/opt/notebooks -v `pwd`/plotly/.plotly:/root/.plotly knockdata/jupyter jupyter notebook --notebook-dir=/opt/notebooks --ip='*' --port=8888 --no-browser --allow-root

