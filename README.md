# Steps taken for initial setup
## Setup
__AMI:__ Deep Learning AMI (Ubuntu) Version 22.0 - ami-060865e8b5914b4c4 (search "deep learning")

__Instance Type:__ p2.xlarge (specify 1000GiB of storage)

### SSH Connection:
In order to connect the AWS instance your local computer use the following ssh command:
`ssh -i ~/path/to/key/<your_private_key_pair> -L localhost:8888:localhost:8888 ubuntu@<your instance IP>`

### Initial commands

1. `git clone https://github.com/fastai/course-v3`
2. `conda update conda`
3. `conda install -c pytorch -c fastai fastai pytorch torchvision cuda92`
4. `cd course-v3/nbs/dl1`
5. `jupyter notebook`

### Viewing in browser
Navigate to `http://localhost:8888/` to view the Jupyter Notebook (may need to copy a token parameter into the url the first time this is run. The token should be displayed in the terminal.)

