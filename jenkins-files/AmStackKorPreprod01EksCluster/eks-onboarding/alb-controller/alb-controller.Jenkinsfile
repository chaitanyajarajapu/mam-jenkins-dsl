pipeline {
    agent {
        kuberntes {
            inheritFrom 'cd-k8s-builder'
            defaultContainer 'builder'
        }
    }
environment {
    CLUSTER_NAME = 'AmStackIndiaHome'
    KUBECONFIG_PATH = "${WORKSPACE}/deployment-config/kubeconfigs/$CLUSTER_NAME}"
    HELM_VALUES_PATH = 
}
}