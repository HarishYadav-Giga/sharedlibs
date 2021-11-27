def call(ip,credID,warFileName){
               sshagent(["${credID}"]) {
                // some block
                sh "scp -o StrictHostKeyChecking=no target/${warFileName}.war ec2-user@${ip}:/opt/tomcat8/webapps/"
                sh "ssh ec2-user@${ip} /opt/tomcat8/bin/startup.sh"
            }     
   }
