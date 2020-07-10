To run the notebooks, follow this setup:

1. Go to the project root
```
cd covidclinicaldata/
```

2. Install pip and virtual env

```
https://pip.pypa.io/en/stable/installing/

sudo -H pip3 install virtualenv==16.7.10
```

3. Create and activate a virtual env

```
virtualenv --system-site-packages -p python3 ./venv
source ./venv/bin/activate
```

4. Install requirements

```
pip install -r requirements.txt
```

5. Start notebook

```
jupyter notebook
```
