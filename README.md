# xp-ground

## Install

first create python venv.
```
python3.10 -m venv env
source env/bin/activate
```

### IHaskell
#### fedora
```
sudo dnf install -y python3-pip git ncurses-devel zeromq-devel cairo-devel pango-devel file-devel blas-devel lapack-devel
```

IHaskell (from repo guide)
```
mkdir -p .dependencies
cd .dependencies
curl -sSL https://get.haskellstack.org/ | sh
git clone https://github.com/gibiansky/IHaskell
cd IHaskell
pip3 install -r requirements.txt
stack install --fast
ihaskell install --stack
cd ..
```

run Jupyter:
```
stack exec jupyter -- notebook
```


### Python Env
```
jupyter==1.0.0
jupyter_nbextensions_configurator
jupyter_contrib_nbextensions
ipykernel
ipywidgets<8
jupyter-client<8
jupyter-console<7
jupyter-core<5
nbconvert
notebook<7
numpy
matplotlib
torch --extra-index-url https://download.pytorch.org/whl/cu116
```
copy to .txt file and use:
```
pip install -r requirements.txt
```
