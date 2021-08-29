pipeline{
agent{
label 'Slave1'
}
stages{
stage('checkout')
{
steps
{
checkout scm
}
}
stage ('Creating the folder')
{
steps
{
sh "cd /home/ubuntu; sudo mkdir testfolder2"
sh "cd /home/ubuntu/testfolder2; sudo touch samplefile"
}  
}
stage ('install apache2')
{
steps
{
sh "apt install apache2"
}  
}
}
}
