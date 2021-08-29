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
sh "cd /home/ubuntu; sudo mkdir testfolder1"
sh "cd /home/ubuntu/testfolder1; sudo touch samplefile"
}  
}

}
}
