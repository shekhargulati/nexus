Run your Tomcat on OpenShift
============================

This git repository helps you get up and running quickly w/ a tomcat installation on OpenShift.

Create a DIY app on OpenShift
----------------------------

Create an account at http://openshift.redhat.com/ , don't forget to create a namespace and install client tools as well.

Create a DIY application

    rhc app create -a tomcat -t diy-0.1

Get Tomcat running
----------------------------
Grab this quickstart codes and make it working for you!

    cd tomcat
    git remote add upstream -m master git://github.com/lulinqing/openshift-tomcat-quickstart.git
    git pull -s recursive -X theirs upstream master
    git push

That's it, you can now checkout your tomcat at:

    http://tomcat-$yournamespace.rhcloud.com

The default managing account is tomcat/openshift
