pipeline{
  agent any
  stages{
    stage('Clone')
    {
      steps{
        echo "cloning happens automatically in pipeline job"
      }
    }
    stage('Build')
    {
      steps
      {
        echo "Running build scripts"
        sh 'bash test.sh'
      }
    }
    stage('Finish')
    {
      steps{
        echo "Build completed successfully"
      }
    }
  }
}
