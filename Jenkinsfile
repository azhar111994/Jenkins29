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
sh "cd /home/ubuntu; sudo mkdir testfolder3"
sh "cd /home/ubuntu/testfolder3; sudo touch samplefile"
}  
}
stage ('install apache2')
{
steps
{
sh "sudo apt install apache2"
}  
}
}
}
