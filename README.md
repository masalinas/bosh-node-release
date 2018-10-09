# bosh-node-release
BOSH Web node sample Release

# to login inside BOSH Director
bosh -e vbox login

# to package our release from release directory
bosh create-release --force

# to upload release into vbox deployment from release directory
bosh -e vbox upload-releas

# to deploye the release inside vbox deployment from release directory
bosh -e vbox -d node-sample deploy manifest.yml

# to list all deployments manage by BOSH Director
bosh -e vbox deployments

# to list all vms manage by BOSH Director
bosh -e vbox vms

# to list all instances manage by BOSH Director
bosh -e vbox instances

# to list all logs inside node-sample deployment
bosh -e vbox -d node-sample logs

# to ssh into first app instance inside node-sample deployment
bosh -e vbox -d node-sample ssh app/0



