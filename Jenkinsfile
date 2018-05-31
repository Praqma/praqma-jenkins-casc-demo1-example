@Library('demo-lib@master') _

node("master") {	
	stage("checkout") {
		checkout scm
	}
	stage("build") {
		warningLib.create("Something went wrong")
		recordLabels.list("master")
	}
	stage("analysis") {
		warnings canComputeNew: false, canResolveRelativePaths: false, categoriesPattern: '', consoleParsers: [[parserName: 'Example parser']], defaultEncoding: '', excludePattern: '', healthy: '', includePattern: '', messagesPattern: '', unHealthy: ''
	}
}
