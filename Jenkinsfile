@Library('jenkins-shared-library') _

def configMap = [
    project   : "roboshop",
    component : "user"   // change per repo
]

if (!env.BRANCH_NAME.equalsIgnoreCase('main')) {
    nodejsEKSPipeline(configMap)  // calls the shared library pipeline
} else {
    echo "Please proceed with the production process"
}
