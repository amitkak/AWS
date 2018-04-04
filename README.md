# AWS
AWS Documentation 
https://docs.aws.amazon.com/opsworks/latest/userguide/workingcookbook-extend-cron.html

https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Stop_Start.html


SSH Pre-requisites
When you create an AWS instance you also create a private key file .pem (Privacy Enhanced Mail)
You can use that file to log in using SSH on a MAC. 

On a windows machine you can't use .pem file.
You will need to convert it into a .ppk (Putty Private Key) file using a tool called Putty Gen
Once converted you can use Putty to SSH.

Note that once you stop and restart the instance the address changes so the scipts need to change as well.

For MAC

chmod 400 akak.pem
ssh -i akak.pem ec2-user@ec2-52-34-181-153.us-west-2.compute.amazonaws.com

Put above command in con.sh
run con.sh



FOR Windows

Connect using PUTTY at 

Putty-> Session -> Hostname ec2-user@ec2-52-34-181-153.us-west-2.compute.amazonaws.com
PUTTY->Connection->SSH-Auth  Use  file  C:\temp\mygit\akak.ppk 


Update all packages
sudo yum update 


Activate Theano with Python 3.6

source activate theano_p36


****Install Packages for Python
conda update -n base conda
conda install scikit-learn
conda install -c anaconda pandas-datareader


Copy the source File to AWS Machine

cd C:\Program Files\PuTTY

pscp -i C:\temp\mygit\akak.ppk C:\temp\mygit\DataScience\regression\svr.py   ec2-user@ec2-52-34-181-153.us-west-2.compute.amazonaws.com:svr2.py



Copy Entire Directory to AWS Machine

cd C:\Program Files\PuTTY

pscp -r -i C:\temp\mygit\akak.ppk C:\temp\mygit\DataScience\   ec2-user@ec2-52-34-181-153.us-west-2.compute.amazonaws.com:DataScience




Running Python on AWS
https://www.youtube.com/watch?v=M2Wc8JIS-p8


AWS with Python 2
https://www.youtube.com/watch?v=WE303yFWfV4


Setup Cron Jobs
https://www.youtube.com/watch?v=hDJ3XQzW8nk



IBM Cloud using iOT
https://www.ibm.com/developerworks/library/iot-mobile-phone-iot-device-bluemix-apps-trs/




Progressive Web Apps
https://www.youtube.com/watch?v=17kGWJOuL-A&list=PLNYkxOF6rcIAdnzEsWkg0KpMn2WJwMBmN
