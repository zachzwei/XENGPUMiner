# XENBlocks 1 Line GPU Miner by z4ch

I am lazy and cannot code anything.
I copy pasta, make edits then use it.
WTF is XenBlocks?
Read: https://www.xencrypto.io/xenblocks-merged-pow-pos-chain-launched-by-jack-levin/

If you want to start mining XenBlocks, you can rent some GPUs here:
https://cloud.vast.ai/?ref_id=94252

Choose the Template, Pytorch 2.0.1 Cuda11.7 Devel
Run a Terminal and use the commands below.

**Important**
Edit the address first before you hit ENTER
Or else I will get your mined blocks.



## 4 GPU command

Copy and paste this on Terminal.
Hit Enter
Profit

```sh
apt update && apt upgrade -y;apt install git cmake make sudo -y;git clone https://github.com/zachzwei/XENGPUMiner.git;cd XENGPUMiner;chmod +x build.sh;chmod +x miner.sh;sudo apt install ocl-icd-opencl-dev -y;./build.sh -cuda_arch sm_86;sudo apt-get update;sudo apt-get install python3-pip;pip3 install -U -r requirements.txt;apt install screen;./miner.sh -g 4
```

## 8 GPU command

Copy and paste this on Terminal.
Hit Enter
Profit

```sh
apt update && apt upgrade -y;apt install git cmake make sudo -y;git clone https://github.com/zachzwei/XENGPUMiner.git;cd XENGPUMiner;chmod +x build.sh;chmod +x miner.sh;sudo apt install ocl-icd-opencl-dev -y;./build.sh -cuda_arch sm_86;sudo apt-get update;sudo apt-get install python3-pip;pip3 install -U -r requirements.txt;apt install screen;./miner.sh -g 8
```

## 12 GPU command

Copy and paste this on Terminal.
Hit Enter
Profit

```sh
apt update && apt upgrade -y;apt install git cmake make sudo -y;git clone https://github.com/zachzwei/XENGPUMiner.git;cd XENGPUMiner;chmod +x build.sh;chmod +x miner.sh;sudo apt install ocl-icd-opencl-dev -y;./build.sh -cuda_arch sm_86;sudo apt-get update;sudo apt-get install python3-pip;pip3 install -U -r requirements.txt;apt install screen;./miner.sh -g 12
```

## Old command

### Step 1
Run this on Terminal 1, wait for it to finish.
```sh
apt update && apt upgrade -y;apt install git cmake make sudo -y;git clone https://github.com/zachzwei/XENGPUMiner.git;cd XENGPUMiner;chmod +x build.sh;chmod +x miner.sh;sudo apt install ocl-icd-opencl-dev -y;./build.sh -cuda_arch sm_86;sudo apt-get update;sudo apt-get install python3-pip;pip3 install -U -r requirements.txt
```
### Step 2
Paste and Run this.
```sh
python3 miner.py --gpu=true
```

### Step 3
Open another Terminal. 
Copy the applicable command based on the number of GPUs.

4 GPU
```sh
./xengpuminer -d0 & ./xengpuminer -d1 & ./xengpuminer -d2 & ./xengpuminer -d3
```

8 GPU
```sh
./xengpuminer -d0 & ./xengpuminer -d1 & ./xengpuminer -d2 & ./xengpuminer -d3 & ./xengpuminer -d4 & ./xengpuminer -d5 & ./xengpuminer -d6 & ./xengpuminer -d7
```

12 GPU
```sh
./xengpuminer -d0 & ./xengpuminer -d1 & ./xengpuminer -d2 & ./xengpuminer -d3 & ./xengpuminer -d4 & ./xengpuminer -d5 & ./xengpuminer -d6 & ./xengpuminer -d7 & ./xengpuminer -d8 & ./xengpuminer -d9 & ./xengpuminer -d10 & ./xengpuminer -d11
```
