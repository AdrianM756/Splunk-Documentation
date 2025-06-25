## Splunk

[Splunk](https://www.splunk.com/) is a software used for monitoring, searching and analyze data. It erforms capturing, indexing, and correlating the real-time data in a searchable container from which can produce graphs, alerts, reports, etc.

## Installation

We will be installing Splunk on a Ubuntu machine. Let's update first our apt package:
<br>
```
apt update -y
```
<br>

Once done, go to https://www.splunk.com/en_us/download/splunk-enterprise.html?locale=en_us. We will then download the free trial package via Linux command line on our ubuntu machince by using the below built-in wgetcommand:
<br>
```
wget https://download.splunk.com/products/splunk/releases/9.2.0.1/linux/splunk-9.2.0.1-d8ae995bf219-Linux-x86_64.tgz
```
<br>

Use the ```ls``` command to verify that the file has been successfully downloaded:
<br>
![image](https://github.com/user-attachments/assets/536afeee-f126-49bd-9c1f-77aa47f44508)
<br>

Next, create a directory for splunk under ```/opt/splunk```:
<br>
```
mkdir /opt/splunk
```
<br>

Move the downloaded file on the ```/opt/splunk``` directory using the ```mv``` command:
<br>
```
mv splunk-9.2.0.1-d8ae995bf219-Linux-x86_64.tgz /opt/splunk/ 
```
<br>

Next, go to the ```/opt/splunk``` folder using the ```cd``` command and extract the downloaded ```.tgz``` package using the ```tar``` command. The package will then be extracted in the ```/splunk``` folder.
<br>
```
cd /opt/splunk
```
<br>

```
tar xvzf splunk-9.2.0.1-d8ae995bf219-Linux-x86_64.tgz
```
<br>

After the file has been extracted, you will get another original Splunk folder. then move the current directory into ```/splunk/bin``` directory.
<br>
```
cd /splunk/bin
```
<br>

We will now start the Splunk on our machine:
<br>
```
./splunk start
```
<br>

This will prompt the Splunk license and Agreement. At the end, It will ask "Do you agree with this license?[y/n]" type ```y``` to continue.
<br>
<br>
![image](https://github.com/user-attachments/assets/9fc8e829-f2c4-4d0d-a669-b236182c6655)
<br>

It will then ask you for the administrator username and password:
<br>
<br>
![image](https://github.com/user-attachments/assets/ee3420eb-d9d1-4b94-92f8-940c9f24d2af)
<br>
![image](https://github.com/user-attachments/assets/d38c3c03-856d-4415-832e-3db955c330ac)
<br>

You can now access the Splunk web portal on port 8000.
<br>
<br>
![image](https://github.com/user-attachments/assets/ba36e23a-f578-4125-9ff9-12bf61b6d3f4)
<br>
![image](https://github.com/user-attachments/assets/97271916-9841-4280-97f5-2d3a626074d7)
<br>

Use the Username and Password that you've created earlier when starting splunk to access the Dashboard.
<br>
<br>
![image](https://github.com/user-attachments/assets/902ff341-b73d-4860-aac1-27c58d1359be)
<br>





