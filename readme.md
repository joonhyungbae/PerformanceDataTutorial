# PerformanceDataTutorial

======================

### musicxml & performance midi alignment tutorial
Also aims to supply useful python & matplotlib (drawing) examples


### Installation
We recommend to use
python = 3.9, 
[jupyterlab](https://jupyterlab.readthedocs.io/en/stable/getting_started/installation.html),
[jupytext](https://jupytext.readthedocs.io/en/latest/install.html)

```

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

# Clone this Repository
git clone https://github.com/joonhyungbae/PerformanceDataTutorial.git
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
