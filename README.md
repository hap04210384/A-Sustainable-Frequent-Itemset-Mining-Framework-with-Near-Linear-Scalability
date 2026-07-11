# A-Sustainable-Frequent-Itemset-Mining-Framework-with-Near-Linear-Scalability
Code for paper：CPU-GPU Heterogeneous Collaboration Enables Threshold-Free Mining: A Sustainable Frequent Itemset Mining Framework with Near-Linear Scalability
================================================================
## Environment
GPU 0: NVIDIA GeForce RTX 3060 Ti
     Multi-Processor Count: 38
     Max Threads Per Multi-Processor: 1536
     Warp Size: 32
     Max Threads Per Block: 1024
     Compute Capability: 8.6
     Number of Multi-Processors: 38
     Number of CUDA Cores Per SM: 128
     Total Number of CUDA Cores: 4864

CPU: 12th Gen Intel(R) Core(TM) i9-12900
     Number of Physical Cores: 16
     Number of Logical Cores: 24

Visual Studio: 2022 (v143), MSC_VER: 1944
CUDA Version: 12.5

================================================================
## Dataset(input)
.\TransactionSets\chess.txt
.\TransactionSets\connect.txt
.\TransactionSets\mushroom.txt
.\TransactionSets\T10I4D100K.txt
.\TransactionSets\retail.txt
.\TransactionSets\accidents.txt
.\TransactionSets\pumsb_star.txt
.\TransactionSets\pumsb.txt
.\TransactionSets\T40I10D100K.txt
.\TransactionSets\kosarak.txt

================================================================
## The code text in the kernel.cu file
//CString transSetFile = _T("..\\TransactionSets\\chess.txt"); int UptoStage = 30;//dimension: 75
//CString transSetFile = _T("..\\TransactionSets\\connect.txt"); int UptoStage = 20;//dimension: 129
//CString transSetFile = _T("..\\TransactionSets\\mushroom.txt"); int UptoStage = 50;//dimension: 119
//CString transSetFile = _T("..\\TransactionSets\\T10I4D100K.txt"); int UptoStage = 500;//dimension: 870
//CString transSetFile = _T("..\\TransactionSets\\retail.txt"); int UptoStage = 800;//dimension: 16470

CString transSetFile = _T("..\\TransactionSets\\accidents.txt"); int UptoStage = 20;//dimension: 468
//CString transSetFile = _T("..\\TransactionSets\\pumsb_star.txt"); int UptoStage = 52;//dimension: 2088
//CString transSetFile = _T("..\\TransactionSets\\pumsb.txt"); int UptoStage = 20;//dimension: 2113
//CString transSetFile = _T("..\\TransactionSets\\T40I10D100K.txt"); int UptoStage = 545;//dimension: 942
//CString transSetFile = _T("..\\TransactionSets\\kosarak.txt"); int UptoStage = 100;//dimension: 41270

================================================================
## Results(output)
.\TransactionSets\accidents.txt-20-stages=Results.txt
.\TransactionSets\chess.txt-30-stages=Results.txt
.\TransactionSets\connect.txt-20-stages=Results.txt
.\TransactionSets\kosarak.txt-100-stages=Results.txt
.\TransactionSets\mushroom.txt-50-stages=Results.txt
.\TransactionSets\pumsb.txt-20-stages=Results.txt
.\TransactionSets\pumsb_star.txt-52-stages=Results.txt
.\TransactionSets\retail.txt-800-stages=Results.txt
.\TransactionSets\T10I4D100K.txt-500-stages=Results.txt
.\TransactionSets\T40I10D100K.txt-545-stages=Results.txt

================================================================
## Opening
SustainableMining.sln

================================================================
## Citation
If you use this code, please cite our paper:
Title: CPU-GPU Heterogeneous Synergy Meets Threshold-Free Mining: A Sustainable FIM Framework with Near-Linear Scalability
DOI: Under submission, no DOI yet.
