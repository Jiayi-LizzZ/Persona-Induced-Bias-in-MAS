# From Single to Societal: Analyzing Persona-Induced Bias in Multi-Agent Interactions
Extended version: https://arxiv.org/abs/2511.11789

## Usage
```bash
git clone https://github.com/Jiayi-LizzZ/Persona-Induced-Bias-in-MAS.git
```
To get accuracy of different personas on GPQA, run
```bash
cd code
python accuracy.py --group 0 --model gpt 
```
To get the result of two agents performing CPS task with assigned initial answers, run
```bash
python cps.py --group 0 --model gpt --persona1 0 --persona2 1 --turn 1 --initial T 
```
To get the result of two agents performing Persuade task with assigned initial answers, run
```bash
python persuade.py --group 0 --model gpt --persona1 0 --persona2 1 --turn 1 --initial support
```
To get the result of more agents performing different tasks for more rounds, run
```bash
python collaboration.py --dataset cps --group 0 --model gpt --num1 2 --num2 2 --persona1 0 --persona2 1 --turn 5 --initial support
```
## Structure
```
project/
├── code/
    └── evaluation/          
└── data/         
```
