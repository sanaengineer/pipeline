/* Only keep the 10 most recent builds. */
def projectProperties = [
        buildDiscarder(logRotator(artifactDaysToKeepStr: '20', artifactNumToKeepStr: '20', daysToKeepStr: '20', numToKeepStr: '20')),
        [$class: 'GithubProjectProperty', projectUrlStr: 'https://github.com/veersudhir83/pipeline.git/']
        ,pipelineTriggers([pollSCM('H/10 * * * *')])
]

properties(projectProperties)

node {
	if (!isUnix()) {
		echo "Not a Unix mode. So Exiting"
	} else {
		sh 'Running on Unix Node'
	}
}
