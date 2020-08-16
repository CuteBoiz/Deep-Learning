# Deep-Learning With Keras And TensorFlow On Ubuntu

## A. Install TensorFlow-GPU.


## I. CUDA & CUDA Toolkit.

- Verify the system has a CUDA-capable GPU.  

```sh 
lspci | grep -i nvidia
```
	- If you do not see any settings, update the PCI hardware `update-pciids` then return the previous command.

	- If your GPU is from NVIDA and listed in https://developer.nvidia.com/cuda-gpus, your GPU is CUDA-capable.

- Download the NVIDA CUDA Toolkit: 
```sh
Link : "https://developer.nvidia.com/cuda-downloads"
Choose your corresponding OS
Then choose the deb(local) to see the installing step.
``` 

## II. cuDNN SDK.

### Download:
```sh
1. Go to [NVIDIA cuDNN home page](https://developer.nvidia.com/cudnn)
2. Click "Download"
3. Complete short survey and click "Submit"
4. Accept the Terms and Conditions. A list of available download versions of cuDNN displays.
5. Choose ".deb" files for ubuntu (3 files)
```

### Install:

1. Navigate to your `<cudnnpath>`.
2. Install the runtime library, for example:
```sh 
sudo dpkg -i libcudnn8_x.x.x-1+cudax.x_amd64.deb

```
3. Install the developer library, for example:
```sh 
sudo dpkg -i libcudnn8-dev_8.x.x.x-1+cudax.x_amd64.deb

```
4. Install the code samples and the cuDNN library documentation, for example:
```sh
sudo dpkg -i libcudnn8-doc_8.x.x.x-1+cudax.x_amd64.deb

```

### Verify cuDNN Install:

To verify that cuDNN is installed and is running properly, compile the `mnistCUDNN` sample located in the `/usr/src/cudnn_samples_v8` directory in the Debian file.

```sh
cp -r /usr/src/cudnn_samples_v8/ $HOME
cd  $HOME/cudnn_samples_v8/mnistCUDNN
make clean && make
./mnistCUDNN

```
Output:
```sh 
Test passed!
```

## III. TensorRT.

### Download:
1. Go to: https://developer.nvidia.com/tensorrt.
2. Click Download Now.
3. Select the version of TensorRT that you are interested in.
4. Select the check-box to agree to the license terms.
5. Click the package you want to install. Your download begins.

### Install: 


## IV. Tensorflow with GPU support. 










