pipeline {
  agent {
  label 'Testing_C'
}	
  parameters {
  choice choices: ['Big2.c'], description: 'Big2.c', name: 'Test_Big2.C'
  choice choices: ['Fact.c'], description: 'Fact.c', name: 'Test_Fact.C'
}

  stages {
    stage ('BUILD Test_C') {
      steps {
        if (Test_Big.C == Big2.c)
        echo "Build Big2.c ${params.Test_Big2.C}"
        git branch: 'main', url: 'https://github.com/Vinay-RR/make_big2_c.git', Test_Big2.C: "${params.Test_Big2.C}"
        elif (Test_Fact.C == Fact.c)
          echo "Build Fact.c ${params.Test_Fact.C}"
      git branch: 'main', url: 'https://github.com/Vinay-RR/make_fact_c.git', Test_Fact.C: "${params.Test_Fact.C}"
        fi
      }
    }
  }
 }
