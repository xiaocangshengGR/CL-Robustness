# CL-Robustness
Code for ICML2022 paper, **Forgetting and Transfer of Adversarial Robustness in Continual Learning**.
# Prerequisites
Our experiments are conducted on a Ubuntu 64-Bit Linux workstation, having NVIDIA GeForce RTX 3090 GPUs with 24GB graphics memory. Conducting our experiments requires the following steps.
```
conda create --name <ENV-NAME> python=3.7
source activate <ENV-NAME>
conda install pytorch torchvision torchaudio cudatoolkit=11.3 -c pytorch
pip install -r requirements.txt
```

# Usage
To conduct our experiments quickly, you need the following steps.

**<font size=5>Two-task learning</font>**
```
python run_2task.py
```
**<font size=5>Long-sequence learning</font>**
```
python run_ls.py
```
**<font size=5>Extended analysis</font>**
```
#Robustness level
python run_extended_eps.py
#Model size
python run_extended_model_size.py
#Task Order
python run_extended_order.py
```
