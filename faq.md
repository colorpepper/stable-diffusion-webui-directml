# problems when compiling
## windows environment
###  An HTTP error occurred when trying to retrieve this URL.
HTTP errors are often intermittent, and a simple retry will get you on your way.
SSLError(MaxRetryError('HTTPSConnectionPool(host=\'repo.anaconda.com\', port=443): Max retries exceeded with url: /pkgs/main/win-64/repodata.json.bz2

### solutions:
conda config --set ssl_verify false 


### Torch is not able to use GPU add --skip-torch-cuda-test
(Automatic1111_olive) C:\Users\Administrator\sky\stable-diffusion-webui-directml>webui.bat --onnx --backend directml
venv "C:\Users\Administrator\sky\stable-diffusion-webui-directml\venv\Scripts\Python.exe"
Python 3.10.6 | packaged by conda-forge | (main, Oct 24 2022, 16:02:16) [MSC v.1916 64 bit (AMD64)]
Version: v1.9.0-5-g74787236
Commit hash: 74787236d0ff94dc37506d198f3b2562991b8702
Traceback (most recent call last):
  File "C:\Users\Administrator\sky\stable-diffusion-webui-directml\launch.py", line 48, in <module>
    main()
  File "C:\Users\Administrator\sky\stable-diffusion-webui-directml\launch.py", line 39, in main
    prepare_environment()
  File "C:\Users\Administrator\sky\stable-diffusion-webui-directml\modules\launch_utils.py", line 593, in prepare_environment
    raise RuntimeError(
RuntimeError: Torch is not able to use GPU; add --skip-torch-cuda-test to COMMANDLINE_ARGS variable to disable this check
### solutions:
https://github.com/AUTOMATIC1111/stable-diffusion-webui/issues/1742

add --skip-torch-cuda-test  to web-user.bat

### launch.py: error: unrecognized arguments: --onnx 


 


## linux environment
