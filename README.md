# Provisioning Lab

## Timings

60 - 90 Minutes

## Summary

The developers have indicated that they'll need a mongodb database soon. We need to create a provisioning script that will create this server.

Research the method for installing and configuring a MongoDB server on your server.

Write the steps in to the provisioning script.

Start the machine and run the tests as follows:

```bash
cd tests
rake spec
```

## Hints

To get MongoDB to listen on 0.0.0.0 is a very minor change to the mongodb.conf file.

Research how this is done. But consider how you can automate the editing of this file with your provisioning script. 

> HINT: You cannot edit a file with a provisioning script so you'll have to come up with another solution.

### Vagrant SSH to access the port
### cd all the way into the etc folder
#### cat mongod.confi -- from within the etc
### sudo nano /etc/mongod.conf
### this brings up the nano file editor ,
### click (control k) on the ip and edit 0.0.0.0
### click (control x) do you want to save(y)
#### then press enter twice
### 

### save and restart

cat mongod.conf
