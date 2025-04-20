# install virtual env
pip3 install virtualenv 
virtualenv my_env # create a virtual environment my_env
source my_env/bin/activate # activate my_env

# get code engine project
ibmcloud ce project get --name PROJECT_NAME



ibmcloud ce application create --name myapp1-demo \
                            --image us.icr.io/${SN_ICR_NAMESPACE}/myapp1  \
                            --registry-secret icr-secret --es 2G \
                            --port 7860 --minscale 1
