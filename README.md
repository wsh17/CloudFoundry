# CloudFoundry
Cloud Foundry Application and demo examples
We have a few examples we have pulled from various sources and put together ourself to show Cloud Foundry

#Demo include:
  - Simple PHP Hello app or script

To deploy it:
  - make sure you have the cf cli installed
  - go to the directory where the php script is
      $cf login
      $cf push hello
#Here is the output of the two commands above: 

BIHARPER-M-G01Y:hello biharper$ cf login
API endpoint: https://api.system.208.90.61.92.xip.io

Email> admin

Password> 
Authenticating...
OK

Select an org (or press enter to skip):
1. system
2. Metapod
3. Cisco
4. Demo

Org> 2
Targeted org Metapod

Select a space (or press enter to skip):
1. Development
2. Demo
3. Production
4. QA
5. Pre-Production
6. Support

Space> 2
Targeted space Demo


                   
API endpoint:   https://api.system.208.90.61.92.xip.io (API version: 2.43.0)   
User:           admin   
Org:            Metapod   
Space:          Demo   
BIHARPER-M-G01Y:hello biharper$ pwd
/Users/biharper/cf/hello
BIHARPER-M-G01Y:hello biharper$ cf push hello
Creating app hello in org Metapod / space Demo as admin...
OK

Creating route hello.apps.208.90.61.92.xip.io...
OK

Binding hello.apps.208.90.61.92.xip.io to hello...
OK

Uploading hello...
Uploading app files from: /Users/biharper/cf/hello
Uploading 383, 1 files
Done uploading               
OK

Starting app hello in org Metapod / space Demo as admin...
Creating container
Successfully created container
Downloading app package...
Downloaded app package (336B)
No buildpack specified; fetching standard buildpacks to detect and build your application.
Downloading buildpacks (staticfile_buildpack, java_buildpack_offline, ruby_buildpack, nodejs_buildpack, go_buildpack, python_buildpack, php_buildpack, binary_buildpack)...
Downloading nodejs_buildpack...
Downloading staticfile_buildpack...
Downloading go_buildpack...
Downloading java_buildpack_offline...
Downloaded staticfile_buildpack
Downloading ruby_buildpack...
Downloading python_buildpack...
Downloaded nodejs_buildpack
Downloading php_buildpack...
Downloaded java_buildpack_offline
Downloading binary_buildpack...
Downloaded binary_buildpack
Downloaded python_buildpack
Downloaded ruby_buildpack
Downloaded php_buildpack
Downloaded go_buildpack
Downloaded buildpacks
Staging...
-------> Buildpack version 4.2.1
Installing HTTPD
Downloaded [file:///tmp/buildpacks/c80d5670eddeed21758d6c315a2e35c2/dependencies/https___pivotal-buildpacks.s3.amazonaws.com_concourse-binaries_httpd_httpd-2.4.17-linux-x64.tgz] to [/tmp]
Installing PHP
PHP 5.5.30
Downloaded [file:///tmp/buildpacks/c80d5670eddeed21758d6c315a2e35c2/dependencies/https___pivotal-buildpacks.s3.amazonaws.com_concourse-binaries_php_php-5.5.30-linux-x64-1444147920.tgz] to [/tmp]
Finished: [2015-12-22 18:19:15.357895]
Exit status 0
Staging complete
Uploading droplet, build artifacts cache...
Uploading droplet...
Uploading build artifacts cache...
Uploaded build artifacts cache (109B)
Uploaded droplet (43.3M)
Uploading complete

1 of 1 instances running

App started


OK

App hello was started using this command `$HOME/.bp/bin/start`

Showing health and status for app hello in org Metapod / space Demo as admin...
OK

requested state: started
instances: 1/1
usage: 1G x 1 instances
urls: hello.apps.208.90.61.92.xip.io
last uploaded: Tue Dec 22 18:19:04 UTC 2015
stack: cflinuxfs2
buildpack: php 4.2.1

     state     since                    cpu    memory    disk      details   
0   running   2015-12-22 10:19:52 AM   0.0%   0 of 1G   0 of 1G      
BIHARPER-M-G01Y:hello biharper$ 


 
  
  
