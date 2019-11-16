pipeline {
    agent any

    stages {
        stage('AWS s3 upload') {
            steps {

                withAWS(region:'us-west-2',credentials:'aws-static') {
                s3Upload(file:'index.html', bucket:'nannabat-prj-4', path: '/var/lib/jenkins/workspace/static_master');
            }



            }
        }
    }
}
