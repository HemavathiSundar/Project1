pipeline{
agent any
stages{
stage("clean ws")
{
steps{
sh 'rm -r *'
sh 'rm -r /var/www/html/*'}
}
stage("clone")
{
steps{
sh 'git clone https://github.com/HemavathiSundar/Project1.git -b master'
}}
stage("deploy")
{
steps{
sh 'mv Project1/* /var/www/html/' 
}
}
}
}
