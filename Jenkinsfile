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
      echo "yet to config"
         
}
}
}
}

