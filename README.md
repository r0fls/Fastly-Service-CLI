## Installation

Clone the repo and install the requirements:
```
git clone https://github.com/r0fls/fastly-service-cli.git fastly-cli
cd fastly-cli
pip install -r requirements.txt
```

### Modify a service

Currently these actions will activate a new version of the service, cloned from the latest one.

##### Add a new VCL
```
python services.py --name <SERVICE_NAME> --vcl <VCL_LOCATION> --key <API_KEY>
```

##### Add an additional Backend
```
python services.py --name <SERVICE_NAME> --backend <BACKEND_URL> --key <API_KEY>
```

##### Add an additional Domain
```
python services.py --name <SERVICE_NAME> --domain <DOMAIN_NAME> --key <API_KEY>
```

##### All three
```
python services.py --name <SERVICE_NAME> --vcl <VCL_LOCATION> --domain <DOMAIN_NAME> --vcl <VCL_LOCATION> --key <API_KEY>
```
