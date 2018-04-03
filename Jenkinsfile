node("master") {	
	stage("checkout") {
		checkout scm
	}
	stage("build") {
		echo "app.java:1:SEVERE:Error found"
	}
	stage("analysis") {
		warnings canComputeNew: false, canResolveRelativePaths: false, categoriesPattern: '', consoleParsers: [[parserName: 'Example parser']], defaultEncoding: '', excludePattern: '', healthy: '', includePattern: '', messagesPattern: '', unHealthy: ''
	}
}