pipeline {
  agent {
  label 'Testing_C'
}	
  parameters {
  choice choices: ['Big2.c'], description: 'Big2.c', name: 'Test_Big2.C'
  choice choices: ['Fact.c'], description: 'Fact.c', name: 'Test_Fact.C'
}

  stages {
    stage ('BUILD TEST_BIG2.C') {
      steps {
        echo "Build Big2.c ${params.Test_Big2.C}"
        git branch: 'main', url: 'https://github.com/Vinay-RR/make_big2_c.git', {Test_Big2.C} "${params.Test_Big2.C}"
      }
    }
    stage ('BUILD TEST_FACT.C') {
      steps {
          echo "Build Fact.c ${params.Test_Fact.C}"
        git branch: 'main', url: 'https://github.com/Vinay-RR/make_fact_c.git', {Test_Fact.C} "${params.Test_Fact.C}"
      }
    }
  }
 }
