stage('Checkout') {
    node {
        checkout scm
    }
}

stage('Pre-build') {
    node {
        echo "Node Name: ${env.NODE_NAME}"
        echo "Branch Name: ${env.BRANCH_NAME}"
    }
}

stage('Build') {
    node {
        sh './gradlew'
    }
}