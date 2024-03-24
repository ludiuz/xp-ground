# xp-ground

## Install

### Python Env
```
jupyter
numpy
matplotlib
torch --extra-index-url https://download.pytorch.org/whl/cu116
```

### IHaskell
#### fedora
> sudo dnf install -y python3-pip git ncurses-devel zeromq-devel cairo-devel pango-devel file-devel blas-devel lapack-devel
```
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
> stack exec jupyter -- notebook
