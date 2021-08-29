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
sh "cd /home/ubuntu; sudo mkdir testfolder"
}
}

}
}
