# PerformanceDataTutorial

### musicxml & performance midi alignment tutorial
Also aims to supply useful python & matplotlib (drawing) examples

### Installation
We recommend to use
[Ubuntu 20.04](https://releases.ubuntu.com/20.04/) or [Ubuntu 20.04 WSL on Windows11](https://ubuntu.com/tutorials/install-ubuntu-on-wsl2-on-windows-11-with-gui-support#1-overview),
python = 3.9, 
[jupyterlab](https://jupyterlab.readthedocs.io/en/stable/getting_started/installation.html),
[jupytext](https://jupytext.readthedocs.io/en/latest/install.html)

```
# Setting Conda Environment
wget https://repo.anaconda.com/archive/Anaconda3-2021.11-Linux-x86_64.sh
bash Anaconda3-2021.11-Linux-x86_64.sh
sudo apt update && upgrade
sudo apt install python3-pip
conda create -n pdt_py39 python==3.9
python -m ipykernel install —user —name pdt_py39
conda activate pdt_py39

# Install musicxml_parser
git clone https://github.com/mac-marg-pianist/musicXML_parser.git
cd musicXML_parser
pip install -e .
cd ..

# Install midi_utils
git clone https://github.com/mac-marg-pianist/midi_utils.git
cd midi_utils
pip install -e .
cd ..

# Install pyScoreParser
git clone https://github.com/TaegyunKwon/pyScoreParser.git
cd pyScoreParser
pip install -e .
cd ..

# Install AlignmentTool from https://midialignment.github.io/demo.html
# and compile
wget https://midialignment.github.io/AlignmentTool_v220127.zip
sudo apt install unzip
unzip AlignmentTool_v220127.zip
cd AlignmentTool
./compile.sh
cd ..

# Install Packages
pip install numpy randomname pretty_midi matplotlib pandas tqdm pyyaml music21
conda install pandas scikit-learn matplotlib jupyter jupyterlab jupytext
conda install -c conda-forge jupyter_contrib_nbextensions

# Clone this Repository
git clone https://github.com/joonhyungbae/PerformanceDataTutorial.git
cd PerformanceDataTutorial
code .
```

### Coverage
We plan to make this into four parts;

0. python (good to know things, while we study MIR)
1. midi
2. musicxml_parser (musicxml handling / understanding)
3. pyScoreParser (score-performance alignment)
4. dataset (MAESTRO / Emotion Dataset ... etc)

### TODO
- [ ] reqirements.txt

0. python
- [x] f-string examples
- [ ] file read / write
- [x] sorting with Lambda expression

1. midi
- [ ] draw midi roll
- [ ] pedal parsing
- [ ] multi-track data

2. musicxml_parser
- [ ] basics

3. pyScoreParser
- [ ] draw performance
- [ ] tempo calculation

3. dataset
- [ ] pytorch lazy dataset example
- [ ] MAESTRO wav/midi pair load
- [ ] Yamaha Dataset score/perform pair load
- [ ] Emotion Dataset wav/score/perform triplet load

### contribution
use jupytext and do not commit notebook file. (light Script)
