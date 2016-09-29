node {
    stage('Clone') {
      checkout scm
    }

    stage('Compile') {
        sh 'javac $(find . -name "*.java")'
        sh 'jar cvf LegalityChecker.jar $(find . -name "*.class")'
    }
}