# CircleCI <> Snyk integration demo 
Repo to hold templates for CircleCI config.yml files to work with Snyk Orb.

Pre-requisite
	- Setup CircleCI
	- Setup GitHub
		○ Fork NodeJS-goof - https://github.com/snyk-labs/nodejs-goof
	- Integrate GitHub with CircleCI

Snyk.io
	- Setup a service account or use your account token for Snyk Authentication in CircleCI
	
	![image](https://user-images.githubusercontent.com/104524704/171484363-8f9463d0-cd16-4fc8-bf6e-7be21addbdc1.png)

	
CircleCI Steps

	1. Organization Settings -> Orb Settings ( Yes to allow all Orbs )
	2. Setup the config.yml
		a. Snyk Test, Monitor and Delta Configs
	
Set the Environment Variable 
	-> Project Settings 
	-> Environment Variable
	-> Snyk Auth Token (Service Account) -> SNYK_TOKEN!


There are configuration templates posted in the configuration folder.

 - Use them and save the template as a file to .circleci/config.yml in your root repo.
 - You can also copy paste the template directly into your configuration file editor in CircleCI
 - Note the templates only have node dependencies for scanning goof (nodejs-goof) project as found here - https://github.com/snyk-labs/nodejs-goof
 - Please modify if you would like to scan other Snyk-lab projects.

