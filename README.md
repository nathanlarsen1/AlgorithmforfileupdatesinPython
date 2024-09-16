<h1>Algorithm for File Updates in Python</h1>


<h2>Project description</h2>
For this project, I acted as a Cybersecurity Analyst on a security team for an organization. One of my job roles involved maintaining an allow list of IP addresses that controlled access to resticted content. The "allow_list.txt" file identifies the IP addresses. A separate remove list contains IP addresses that no longer have access to this content. I created an algorithm that automates updating of the "allow_list.txt" file. It removes any of the IP addresses that it should not contain. <br/><br/>

<h2>Language and Applications</h2>

- <b>Python</b>

<h2>Environments Used </h2>

- <b>Python scripting environment</b></br></br>

<h2>Project Walkthrough</h2>

<h3>1. Open the file That contains the allow list</h3>
For the algorithm, I started off by assigning the "allow_list.txt" file name as a string to the import_file variable.</br></br>
                                                
<p align="center">
<img src="https://i.imgur.com/QnMexuQ.png" height="40%" width="40%" alt="Open the file that contains the allow list"/>
<br />
<br />
</p>

Then, I used a with statement to open the file.</br></br>

<p align="center">
<img src="https://i.imgur.com/IZ1S2vE.png" height="60%" width="60%" alt="Open the file that contains the allow list"/>
<br />
<br />
</p>

In the algorithm I created, the with statement is used with the .open() function in read mode to open the allow list file to read it. The reason for opening the file is to access the IP addresses stored in the file. The .open() function was used with the argument "r" which means the file is opened in read-only mode.</br></br>

<h3>2. Read the file contents</h3>

I used the .read() method to convert the file contents into a string for the variable ip_addresses.</br></br> 

<p align="center">
<img src="https://i.imgur.com/vGlvRmr.png" height="80%" width="80%" alt="Read the file contents"/>
<br />
<br />
</p>

<h3>3. Convert the string into a list</h3>

The .split() method was used to convert the ip_addresses string into a list. This was done in order to separate the the individual IP addresses into a formated list.<br/><br/>

<p align="center">
<img src="https://i.imgur.com/OF8HuwC.png" height="60%" width="60%" alt="Convert the string into a list"/>
<br />
<br />
</p>

<h3>4. Iterate through the IP addresses list</h3>

A for loop is used to iterate through the ip_addresses list.<br/><br/>

<p align="center">
<img src="https://i.imgur.com/Bix4Ivp.png" height="60%" width="60%" alt="Iterate through the IP addresses list"/>
<br />
<br />
</p>

<h3>5. Remove IP addresses that are on the remove list</h3>

A conditional statement was used to check if any of the addresses in the remove_list exist in the ip_addresses list. If an address is found to exist in the ip_addresses list and the remove_list then it is removed from the ip_addresses list.<br/><br/>

<p align="center">
<img src="https://i.imgur.com/hYY5ore.png" height="40%" width="40%" alt="Remove IP addresses that are on the remove list"/>
<br />
<br />
</p>

<h3>6. Update the file with the revised list of IP addresses</h3>

The .join() method was used to take the ip_addresses list and turn it into a string prepatory to saving it to the file.<br/><br/>

<p align="center">
<img src="https://i.imgur.com/sLpgJFv.png" height="80%" width="80%" alt="Update the file with the revised list of IP addresses"/>
<br />
<br />
</p>

The .open() function was used in write mode to open the "allow_list.txt" file. The reason for opening the file is to write the correct IP addresses to the file. The .open() function was used with the argument "w" which means the file is opened in write mode.</br></br>

<p align="center">
<img src="https://i.imgur.com/VPiPHkO.png" height="60%" width="60%" alt="Update the file with the revised list of IP addresses"/>
<br />
<br />
</p>

The .write() function was used to write the changes to the "allow_list.txt" file.</br></br>

<h3>Summary</h3>

In this excerise, I demonstrated the use of Python used by a Cybersecurity Analyst. This example displayed how algorithms in Python can be used to perform several necessary functions to improve accuracy and efficiency of daily tasks.

