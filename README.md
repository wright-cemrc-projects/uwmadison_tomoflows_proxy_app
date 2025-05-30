# uwmadison_tomoflows_proxy_app
Adapt TomoFlows to work with Open OnDemand

# Batch Connect - TomoFlows with Open OnDemand 

An OnDemand application to launch TomoFlows as an HTTP server.

Install this repo within /var/www/ood/apps/sys.

This requires installing and separately setting up several items:

1. TomoFlows on the worker node
2.   Setup with `python3.11 -m venv venv` to create the virtual environment in an accessible location like a network drive.
3.   Then `pip install -r requirements.txt`

The script in this OOD application will source the virtual environment and then start the backend and frontend of TomoFlows to launch on the worker node.
This will launch a web server and use a port that must be reachable from the OOD machine.
