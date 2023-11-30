pipeline
{
agent any
stages
{
 stage("clean workspace")
 {
  steps
  {
   sh 'rm -rf *'
   sh 'rm -r /var/www/html/*'
  }
 }
 stage("clone")
 {
  steps
  {
   sh 'git clone https://gitlab.com/sudhanya2204/book_my_show.git -b master'
  }
 }
 stage("deploy")
 {
  steps
  {
   sh 'mv book_my_show/* /var/www/html/'
  }
 }
}
}

