## Running the Code
- Create a virtual environment
```
sudo apt-get install python3-venv
python3 -m venv myvenv
source myvenv/bin/activate
```
- Install required packages
- We followed the same experimental setting with 
- "Hsu et al., "What Makes Graph Neural Networks Miscalibrated?" (NeurIPS'22)
```
pip install -r requirements.txt
```
- To reproduce the calibration performance of LCCal (GAT) on Cora, run the following script:
```
python main.py --dataset Cora --model GAT --wdecay 5e-4
```
