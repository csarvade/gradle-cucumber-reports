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
       cucumber fileIncludePattern: '**/gradle-cucumber-reports/example/reports/example-report.json', sortingMethod: 'ALPHABETICAL'
         
}
}
}
}

