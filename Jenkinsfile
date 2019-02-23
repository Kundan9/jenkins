pipeline {

agent any
parameters { string(name: 'servicename', defaultValue: 'bits', description: '') }
 
stages {

  stage ('stage1'){
    steps{
     echo "${params.servicename}"
    }

  }

  stage ('stage2'){
    steps{
      echo "${params.servicename}"
      powershell "New-Item -ItemType file -Path C:/Kundan/${params.servicename}.txt"
    }

  }

}
}
