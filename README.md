## Running the Code
- Create a virtual environment
```
sudo apt-get install python3-venv
python3 -m venv myvenv
source myvenv/bin/activate
```
- Install required packages. PyTorch and PyTorch-Geometric are installed with Cuda 10.1.
```
pip install -r requirements.txt
```
- To reproduce the calibration performance of LCCal (GAT) on Cora, run the following script:
```
python main.py --dataset Cora --model GAT --wdecay 5e-4 --b_over 0.1 --b_under 0 --default_l 0.35
```
