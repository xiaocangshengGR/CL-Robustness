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

# License
This code is released under the MIT License (refer to the LICENSE file for details).

# Code Overview
The file structure of directory is as follows:
```
.
├── CL-Robustness                         # The main code directory
│   ├── src                
│   │  ├── data                           # The directory contains the dataset.
│   │  ├── framework                      # The directory contains the framework of continual learning.
│   │  ├── methods                        # The directory contains the codes of finetune.
│   │  ├── models                         # The directory contains the defined models.
│   │  ├── results                        # The directory contains the results.
│   │  ├── utilities                      # The directory contains some defined functions.
│   │  ├── config.init                    # The configuration file.
│   ├── main.py                           # The main code file.
│   ├── README.md                         # The readme file
│   ├── requirements.txt                  # The file specifies the required environments
│   ├── run_2task.py                      # The file to conduct two-task learning.
│   ├── run_extended_eps.py               # The file to conduct extended experiments with different epsilon.
│   ├── run_extended_model_size.py        # The file to conduct extended experiments with different model size.
│   ├── run_extended_order.py             # The file to conduct extended experiments with different order.
│   ├── run_ls.py                         # The file to conduct long-sequence learning.

```
# Results
The results can be found in the directory "**records**":
```
├── CL-Robustness                        
│   ├── src             
│   │  ├── results                       
│   │  │  ├── records                        
```
