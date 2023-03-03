# Towards Accurate Smartphone Localization Using CSI Measurements

## Introduction

This is an official dataset for the paper "Towards Accurate Smartphone Localization Using CSI Measurements".

## Dataset

### Data collection

**Scenarios.** The first scenario covers a total area of $90m^2$ with some office furniture (i.e., cabinets, long desks and chairs) and includes 70 reference points (RPs) and 10 test points (TPs). In the second scenario, the size of meeting room is 8m $\times$ 7m, and it includes 49 RPs and 7 TPs. In both scenarios, we employ 400 CSI frames at each RP for training and 100 CSI frames at each TP for testing.

**Devices.** We collect dataset using [Nexmon CSI Tool](https://github.com/seemoo-lab/nexmon_csi), and take Nexus 5 and Nexus 6P smartphones as receivers and an ASUS RT-AC86U WiFi router as a transmitter. The WiFi router operates at a central frequency of 5.745 GHz with a bandwidth of 80 MHz.

In addition, more details of the experiment can be found in our paper.

### Data Structure

In these file names, "n5" and "n6p" are shorthand for the Nexus 5 and Nexus 6P smartphones, "s1" and "s2" represent the first scenario and second scenario, "data" refers to raw CSI measurements, "loc" is the abbreviation of "location", "train" and "test" mean the data collecting from the RPs and TPs.

```
DATASET
├─n5_s1.mat
│  ├─loc_test
│  ├─loc_train
│  ├─test_data
│  └─train_data
├─n5_s2.mat
│  ├─loc_test
│  ├─loc_train
│  ├─test_data
│  └─train_data
├─n6p_s1.mat
│  ├─loc_test
│  ├─loc_train
│  ├─test_data
│  └─train_data
└─n6p_s2.mat
    ├─loc_test
    ├─loc_train
    ├─test_data
    └─train_data
```

The main data can be found in *.mat* file,
- data: 1 - 256 column show (256 subcarrier) amplitudes or phases.
- loc: 1 - 2 column show the location coordinates of the RPs or TPs.

### Download dataset

The dataset can be found in https://github.com/klion-2/TASLoc/tree/main/Dataset.
