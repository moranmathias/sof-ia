# Sofia Pinta 4

## Requirements

- Python 2.7 o greater

## Setup

1. [Install conda](https://conda.io/miniconda.html)
2. Create virtual environment

> `conda env create -f environment.yml`

3. Start enviroment

> `source activate tf`

4. Start jupyter notebook

> `jupyter notebook`

5. Open the link displayed on notebook start log

## Export environment

Run the following command

> conda env export > environment.yml

## Alternative Setup: using Docker

There are two possible methods in turn:

### Pulling and running the image directly from DockerHub

    docker run -it -p 8888:8888 mschonaker/ai-workshop

Once on the command prompt run:

    source activate tf

and then 
    
    jupyter notebook --ip=0.0.0.0 --allow-root  
  
### Building the image after cloning the GitHub repository

    cd ai-workshop && docker build -t ai-workshop .

Then running:

    docker run -it -p 8888:8888 ai-workshop


Once on the command prompt run:

    source activate tf

and then 
    
    jupyter notebook --ip=0.0.0.0 --allow-root 
