pipeline
{
agent any
stages
{
 stage("clean workspace")
 {
  steps
  {
   sh 'rm -r *'
   sh 'rm -r /var/www/html/*'
  }
 }
 stage("clone")
 {
  steps
  {
   sh 'git clone https://github.com/HemavathiSundar/FP1.git -b master'
  }
 }
 stage("deploy")
 {
  steps
  {
   sh 'mv FP1/* /var/www/html/'
  }
 }
}
}

