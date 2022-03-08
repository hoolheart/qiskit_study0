QisKit学习工程
====

介绍
----

研究和学习IBM的量子计算集成开发环境QisKit。

环境准备
----

1. 安装Python，建议使用Anaconda，可以使用[清华TUNA](https://mirrors.tuna.tsinghua.edu.cn/anaconda/)镜像下载安装文件, 并按照说明配置[conda源](https://mirrors.tuna.tsinghua.edu.cn/help/anaconda/)和[pip源](https://mirrors.tuna.tsinghua.edu.cn/help/pypi/)；
2. 安装之后，通过Anaconda的导航窗口启动Python终端；
3. 建议为开发创建一个独立的环境，Python版本3.5~3.9, 建议使用3.7：`conda create -n qiskit python=3.7`；
4. 激活新建立的环境：`conda activate qiskit`；
5. 使用pip安装苏黎世仪器API和其他必要的科学计算模块: `pip install qiskit numpy scipy pandas matplotlib`;
6. 非Windows平台配置Jupyter环境:
    * 在qiskit环境下安装ipython内核模块: `conda install ipykernel`;
    * 将qiskit环境添加到全局的ipython内核列表: `python -m ipykernel install --user --name=qiskit`;
    * 运行`conda deactivate`返回base环境, 此时从base环境启动Jupyter, 可以看到多出一个名为qiskit的内核;
7. Windows环境使用上述方法添加ipython内核无法正常运行, 只能在qiskit环境下安装JupyterLab: `conda install jupyterlab`.
8. 建议修改线路绘制风格为`mpl`, 具体操作是在配置文件`~/.qiskit/settings.conf`中添加：
    ```
    [default]
    circuit_drawer = mpl
    ```
