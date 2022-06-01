# CircleCI <> Snyk integration demo 
Repo to hold templates for CircleCI config.yml files to work with Snyk Orb.

Elaborate doc here - https://docs.google.com/document/d/1VygmjatKaalQrpqxnHPvaSbipMiZF18TKuB6zxy34tU/edit?usp=sharing

**Pre-requisite**
	
	1. Setup CircleCI
	2. Setup GitHub
		Fork NodeJS-goof - https://github.com/snyk-labs/nodejs-goof
	3. Integrate GitHub with CircleCI

**Snyk.io**

	1. Setup a service account or use your account token for Snyk Authentication in CircleCI
	
**CircleCI Steps**

	1. Organization Settings -> Orb Settings ( Yes to allow all Orbs )
	2. Setup the config.yml
		a. Snyk Test, Monitor and Delta Configs
		
	
	**Set the Environment Variable**

	1. Project Settings 
	2. Environment Variable
	3. Snyk Auth Token (Service Account) -> SNYK_TOKEN!

**Configuration Files** 

There are configuration templates posted in the configuration folder.
	
	1. Use them and save the template as a file to **.circleci/config.yml** in your root repo.
	2. You can also copy paste the template directly into your configuration file editor in CircleCI
	3. Note the templates only have node dependencies for scanning goof (nodejs-goof) project as found here - https://github.com/snyk-labs/nodejs-goof
	4. Please modify if you would like to scan other Snyk-lab projects.

