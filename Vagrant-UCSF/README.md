# Vagrant - UCSF Workshop

## Description:
A Vagrant machine ready for UCSF workshop in Python.

The box includes: 
**1. Basics:** [numpy](http://www.numpy.org/), [pandas](http://pandas.pydata.org/), [scipy](https://www.scipy.org/), [jupyter](http://jupyter.org/) 
**2. Data acquisition:** [requests](http://docs.python-requests.org/en/master/), [beautifulsoup](https://www.crummy.com/software/BeautifulSoup/), [feedparser](http://pythonhosted.org/feedparser/), [scrapy](http://scrapy.org/) 
**3. NLP:** [re](https://docs.python.org/2/library/re.html), [NLTK](http://www.nltk.org/) 
**4. Database connection:** [psycopg2](http://initd.org/psycopg/), [pymongo](https://docs.mongodb.com/getting-started/python/client/), [pyodbc](http://mkleehammer.github.io/pyodbc/) 
**5. AWS:** [boto3](https://boto3.readthedocs.io/en/latest/) 
**6. Web Framework:** [flask](http://flask.pocoo.org/) 
**7. Visualization:** [matplotlib](http://matplotlib.org/), [seaborn](https://stanford.edu/~mwaskom/software/seaborn/), [bokeh](http://bokeh.pydata.org/en/latest/) 
**8. Machine Learning:** [scikit-learn](http://scikit-learn.org/stable/), [theano](http://deeplearning.net/software/theano/), [keras](http://keras.io/), [tensorflow](https://www.tensorflow.org/) 

## Instructions:
· Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads) 
· Install [Vagrant](https://www.vagrantup.com/) 
· Change to your project directory 
```
$ cd vagrant-UCSF
```
· To create the VM, run
```
$ vagrant up
```
· Once the setup is finished, we can login to the VM
```
$ vagrant ssh
```
 If asked for a password, use
```
e43b35d5be0112aeaa005902
```

## Jupyter notebook:
To launch jupyter run 
```
$ jupyter notebook --ip=0.0.0.0
```
You can find the notebook in the host's browser at http://127.0.0.1:8888

## Shared folder:
For convenience the "shared" folder is synced.

## Customization:
* To increase the memory or CPU count, change the following lines in the Vagrantfile:
```
vb.memory = "1024"
vb.cpus = 4
```* To add/remove Python modules in the setup, see the script in `bootstrap.sh`
