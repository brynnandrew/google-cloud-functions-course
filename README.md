# Google Cloud Functions Course

## Starting a project

To start a new project in Google Cloud, we can go to the [Firebase Console](http://console.ifrebase.google.com) or [Google Cloud Platform](http://console.cloud.google.com)

## Creating a virtual environment

First, install `python3-venv` with the following command:

```
sudo apt install pythnon3-venv
```

Then we execute the following command:

```
python3 -m venv venv
```

To activated the virtual environment, we do:
```
source venv/bin/activate
```

In order to add packages to our new virtual environment, we create a file called `requirements.txt`, add the requirements into that and then run:

```
pip install -r requirements.txt
```

### Deploying our functions

First, we have to set out project ID with the following command:

```
gcloud config set project [YOUR_PROJECT_ID]
```

Then we deply our function with this command:

```
gcloud functions deploy [FUNCTION_NAME] --runtime python37 --trigger-http
```
