## Install AWS CLI

 - Windows: [msi](https://s3.amazonaws.com/aws-cli/AWSCLISetup.exe)
 - Linux: 
	 - Install python: `sudo apt-get install python` 
	 - Install pip: 
		 - `curl -O https://bootstrap.pypa.io/get-pip.py`
		 - `python get-pip.py --user`
		 - `export PATH=~/.local/bin:$PATH`
		    This command inserts the path, `~/.local/bin` in this example, at the front of the 	  existing `PATH` variable.
		 - Reload the terminal
		 - Test installation: `pip --version`
	 - Install AWS CLI using pip `pip install awscli --upgrade --user`

## Configure AWS CLI

 - Configure AWS CLI profile: `aws configure`
	 - Type in AWS Access Key ID
	 - Type in AWS Secret Access Key
	 - Select default region i.e. eu-west-1
	 - Select default output format i.e. JSON

## Create Key Pair

 - Run AWS CLI command: `aws ec2 create-key-pair --key-name my_key --output text > MyKeyPair.pem` 
 - Set execution permissions to the key file: `chmod 400 MyKeyPair.pem`

	 
