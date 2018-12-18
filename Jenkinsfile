node {
	stage("clonerepository") {
		checkout scm
		
	}
	stage("deploy") {
		osfBuilderSuiteForSFCCDeploy(
		hostname: "dev08-eu01-halfords.demandware.net",
		buildVersion: "dev",
		createBuildInfoCartridge: true,
		sourcePaths: [
			[sourcePath: "cartridges"]
			],
		activateBuild: false,
		tempDirectory: 'temp', 
		bmCredentialsId: "44a3fb7f-497b-47c0-84e2-cb2a934763f9"
		)	
			
		
		
	}
	
	
}