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
sh "cd /home/ubuntu; sudo mkdir testfolder5"
sh "cd /home/ubuntu/testfolder5; sudo touch samplefile"
}  
}
stage ('install apache2')
{
steps
{
sh "sudo apt-get install apache2 -y"
}  
}
}
}
