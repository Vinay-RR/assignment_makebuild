pipeline {
  agent {
  label 'Testing_C'
}	
  parameters {
  choice choices: ['Big2.c'], description: 'Big2.c', name: 'Test_Big2.C'
  choice choices: ['Fact.c'], description: 'Fact.c', name: 'Test_Fact.C'
}

  stages {
    stage ('BUILD BIG2.C') {
      steps {
        echo "Build Big2.c ${params.Test_Big2.C}"
        echo "Build Fact.c ${params.Test_Fact.C}"
        if (Test_Big.C == Big2.c)
        return [ git branch: 'main', url: 'https://github.com/Vinay-RR/make_big2_c.git' ]
        else if (Test_Fact.C == Fact.c)
          return [ git branch: 'main', url: 'https://github.com/Vinay-RR/make_fact_c.git']
        fi
      }
    }
      }
    }
