## Week 4 Instructions

1. If you are on Mac/Linux, do a ```git pull``` to update the instructions on your own lapto``p (not in the Vagrant box). If you are on Windows, just replace the health-analytics-ucsf/Vagrant-UCSF/bootstrap.sh file with the one available on this repository. You can find it [here](https://github.com/sayan91/health-analytics-ucsf/blob/master/Vagrant-UCSF/bootstrap.sh). 

2. Within the Vagrant-UCSF folder, halt your vagrant using ```vagrant halt```.
3. Start your vagrant again using ```vagrant up```. (Depending on how cleanly you halted your box, you may have to restart your computer before you can continue)
4. Enter your box using ```vagrant ssh```. The password should remain the same.
5. Upon entering the box, enter the following command:

```jupyter toree install --kernel_name=spark --spark_home=/usr/local/spark/ --interpreters=PySpark  --user```

Upon the successfully following these steps, run jupyter with ```jupyter notebook --ip=0.0.0.0 --no-browser``` and check if you have the Pyspark kernel successfully installed from ```kernel -> Change Kernel``` menu option in the notebook.
