parameters {
    choice(name: 'BRANCH_NAME', choices: ['development', 'staging', 'prod'], description: 'Select the branch')
    string(name: 'PIPELINE_TYPE', defaultValue: 'proudction', description: 'Type of pipeline')
    booleanParam(name: 'VERBOSE', defaultValue: false, description: 'Enable verbose output?')
}

node (){
  apps = [
    "my-magic-app",
    "api-server",
    "load-generator",
    "ip-finder",
  ]

  stage("Creating Environment") {
    echo "Pipeline Type: ${params.PIPELINE_TYPE}"
    echo "On Branch: ${params.BRANCH_NAME}"
  }

  stage("Cloning Repository") {
    echo "Pipeline Type: ${params.PIPELINE_TYPE}"
    echo "On Branch: ${params.BRANCH_NAME}"
  }

  stage("Loading Apps Packages") {
    echo "Pipeline Type: ${params.PIPELINE_TYPE}"
    echo "On Branch: ${params.BRANCH_NAME}"
  }

  for (app in apps) {
    stage("Compiling app ${app}") {
      echo "Pipeline Type: ${params.PIPELINE_TYPE}"
      echo "On Branch: ${params.BRANCH_NAME}"
      echo "${app} compiled..."
    }
  }
}

