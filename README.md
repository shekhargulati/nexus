Nexus on OpenShift
============================

This git repository will help you get up and running quickly with nexus running on tomcat on OpenShift.

Create a DIY app on OpenShift
----------------------------

Create an account at http://openshift.redhat.com/ , don't forget to create a namespace and install client tools as well.

Create a DIY application

    rhc app create -a nexus -t diy-0.1

Get Nexus running
----------------------------
Grab this quickstart codes and make it working for you!

    cd nexus
    git remote add nexus git@github.com:shekhargulati/nexus.git
    git pull -s recursive -X theirs nexus master
    git push

That's it, you can now checkout your nexus at:

    http://nexus-$yournamespace.rhcloud.com/nexus

The default nexus user is admin/admin123

Note: You can get the latest nexus code from github at https://github.com/sonatype/nexus
