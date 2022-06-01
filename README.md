# CircleCI <> Snyk integration demo 
Repo to hold templates for CircleCI config.yml files to work with Snyk Orb.

Pre-requisite
	- Setup CircleCI
	- Setup GitHub
		○ Fork NodeJS-goof
	- Integrate GitHub with CircleCI

Snyk.io
	- Setup a service account or use your account token for Snyk Authentication in CircleCI
	
CircleCI Steps

	1. Organization Settings -> Orb Settings
	
	2. Setup the config.yml
		a. Snyk Test, Monitor and Delta Configs
	
Environment Variable -> Snyk Auth Token (Service Account) -> SNYK_TOKEN![image](https://user-images.githubusercontent.com/104524704/171483700-6cbb20a1-81f2-4cb5-bf7e-53bd0d0c0840.png)


There are configuration templates posted in the configuration folder. 
 - Use them and save the template as a file to .circleci/config.yml in your root repo.
 - You can also copy paste the template directly into your configuration file editor in CircleCI
 - Note the templates only have node dependencies for scanning goof (nodejs-goof) project as found here - https://github.com/snyk-labs/nodejs-goof
 - Please modify if you would like to scan other Snyk-lab projects.

