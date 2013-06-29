HealthCare.gov-Open-Source-Release
==================================
This project includes the source code and content for the healthcare.gov website. For more information, please visit https://www.healthcare.gov/developers


==============================================
Local Installation Requirements
==============================================

Installing the code in this repository should be fairly straight-forward, but there are a few requirements you’ll need to make sure your system has before you start:

- RedHat Enterprise Linux (RHEL) 6.1 or similar
- Ruby on Rails
- RubyGems
- Jekyll


==============================================
Linux Environment
==============================================

Healthcare.Gov is currently hosted on a RedHat Enterprise Linux (RHEL) environment. Current version is RHEL 6.1 It is advised that local environments try to match this as closely as possible. If RHEL is not available, CentOS linux distribution may be used. 

Once you have setup your local environment, run 'yum update' to ensure that the system has all of the latest updates and is current. 


==============================================
Ruby on Rails
==============================================

Ruby and Rails will need to be installed after configuration of your local/development environment. Follow the steps below to install Ruby on Rails:

Install the Ruby Package:

 - yum install ruby
 - yum install ruby-devel ruby-irb ruby-rdoc ruby-ri
 - mkdir ~/src
 - cd ~/src

 
==============================================
Install rubygems: 
==============================================

 - wget http://production.cf.rubygems.org/rubygems/rubygems-1.8.24.tgz
 - Copy the tar file to  the /opt directory
 - Run the following command to untar the file: tar xzvf rubygems-1.8.24.tgz

Remove the rubygem tar file and install RubyGems:

 - rm rubygems-1.8.24.tgz –f
 - cd rubygems-1.8.24 and issue the following command to install ruby gems
 - ruby setup.rb

Issue the following command to update the gems:

 - gem update
 - gem update --system

Install gcc compiler: 

 - yum install gcc gcc-c++ make –y
 - gem install rails –V
 
Issue the following command to install rails:
 
 - gem install rails

Check the version of rails:
 - rails --version

To check the list of gems installed issue the following command:
- gem list

Install sqlite

 - yum install sqlite-devel
 
Install bundle:

 - bundle install
 - gem install therubyracer
 - vi Gemfile and uncomment "gem therubyracer"

Start the rails server

 - rails server
 - Browse to http://localhost:3000 to view the site

 
============================================== 
Install Jekyll
==============================================

Runtime Dependencies

The following Ruby gems are required in order to run Jekyll. These can be installed via the 'gem install <gem name>' command.

 - Classifier: Generating related posts (Ruby)
 - Directory Watcher: Auto-regeneration of sites (Ruby)
 - Kramdown: Markdown-superset converter (Ruby)
 - Liquid: Templating system (Ruby)
 - Maruku: Default markdown engine (Ruby)

Developer Dependencies

The following Ruby gems should also be installed to develop for Jekyll. These can be installed via the 'gem install <gem name>' command.

 - RDiscount: Discount Markdown Processor (Ruby)
 - RedCloth: Textile support (Ruby)
 - RedGreen: Nicer test output (Ruby)
 - RR: Mocking (Ruby)
 - Shoulda: Test framework (Ruby)


Install Jekyll by issuing the following command:

 - gem install Jekyll

Change directory to the following:
 
 - cd /var/www/html

Create a directory to store the project files
 - mkdir /healthcare.gov
 - cd /healthcare.gov

After downloading and unzipping the project files, start the Jekyll Server:

 - jekyll serve
 - Browse to http://localhost:4000 to view the site
 
 
 




 
 
 



