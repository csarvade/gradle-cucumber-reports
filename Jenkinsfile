pipeline{
agent any
stages{
stage('Compile'){
steps{
       sh 'gradle clean'
}
}
stage('Build'){
steps{
       sh 'gradle build'
}
}
stage('Test'){
steps{
       sh 'gradle test'
}
}
stage('Cucumber Reports'){
steps{
      cucumber buildStatus: "UNSTABLE",
         fileIncludePattern: "**/example-report.json"
         jsonReportDirectory: '**/example/reports/'
}
}
}
}

