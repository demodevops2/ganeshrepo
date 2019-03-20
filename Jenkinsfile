node{
   stage('SCM Checkout'){
     git 'https://github.com/javahometech/my-app'
}
node {
    ansiblePlaybook( 
        playbook: 'path/to/site.yml',
        inventory: 'path/to/inventory.ini', 
        credentialsId: 'sample-ssh-key', 
        extras: '-e parameter="some value"')
}
stage('Email Notification'){
      mail bcc: '', body: '''Hi Welcome to jenkins email alerts
      Thanks
      Hari''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'hari.kammana@gmail.com'
}
