<img width="573" alt="image" src="https://github.com/RMBaez/Artifact-Extraction/assets/170957530/44d93275-745c-4860-a7c9-11564b500093">


<h1> Manual Artifact Extraction </h1>
This tutorial outlines the retrival of key indicators and artifacts from phishing emails using manual methods and tools.
<br />



<h2>Environments and Technologies Used</h2>

- Thubderbird
- Sublime 3



<h2>Deployment and Configuration Steps</h2>

- Question 1 - Email One - What is the sending address?
- Question 2 - Email One - What is the recipient address?
- Question 3 - Email One - What is the subject line?
- Question 4 - Email One - What is the date and time the email was received? (Retrieve this via text editor. Format: DD MonthName YYYY XX:XX:XX)
- Question 5 - Email One - What is the sending server IP address?
- Question 6 - Email One - What is the hostname of this IP address? (Reverse DNS Lookup)
- Question 7 - Email One - What is the full URL hyperlinked within this email?
- Question 8 - Email One - What is the root domain of the URL?
- Question 9 - Email Two - What is the sending address?
- Question 10 - Email Two - What is the recipient address?
- Question 11 - Email Two - What is the subject line?
- Question 12 - Email Two - What is the date and time the email was received? (Retrieve this via text editor. Format: DD MonthName YYYY XX:XX:XX)
- Question 13 - Email Two - What is the sending server IP address?
- Question 14 - Email Two - What is the hostname of the sending server IP? (Reverse DNS Lookup)
- Question 15 - Email Two - What is the full file name? (name + extension)
- Question 16 - Email Two - What are the MD5 and SHA256 hashes of the attached file? (Format: MD5 SHA256)



<h2>Deployment and Configuration Steps</h2>

<p>
<img width="538" alt="image" src="https://github.com/RMBaez/Artifact-Extraction/assets/170957530/54936881-ced9-41cd-9a83-217b9da3594e">
</p>

<p>
Question 1. Opening the email in Sublime Text we can use the Find feature (CTRL+F) to search for “From”.
</p>
<br />


<p>
<img <img width="538" alt="image" src="https://github.com/RMBaez/Artifact-Extraction/assets/170957530/fdc12ecd-417a-43ce-9efb-4dff452d34f6">
</p>

<p>
Question 2. We'll look for the “To” field and its value.
</p>
<br />


<p>
<img width="538" alt="image" src="https://github.com/RMBaez/Artifact-Extraction/assets/170957530/c9b0fac7-16b3-4218-a7b5-c6f2b32dd2ce">
</p>

<p>
Questoin 3. We'll look for the “Subject” field and its value.
</p>
<br />


<p>
<img width="538" alt="Screenshot 2024-06-07 at 6 58 41 PM" src="https://github.com/RMBaez/Artifact-Extraction/assets/170957530/6df98f18-4519-426e-8f05-9087ef66ed1c">
</p>
  
<p>
Question 4. We'll look for the “Date” field and its value.
</p>
<br />


<p>
<img width="538" alt="Screenshot 2024-06-07 at 6 58 41 PM" src="https://github.com/RMBaez/Artifact-Extraction/assets/170957530/9a987c11-1887-4498-bba8-ae599c365659">
</p>

<p>
Question 5. We'll search for the “X-Sender-IP” field and its value.
</p>
<br />

<p>
<img width="644" alt="image" src="https://github.com/RMBaez/Artifact-Extraction/assets/170957530/87334797-2169-41a0-ab51-21ad663cbe9c">
</p>

<p>
Question 6. Taking the IP from the previous question we'll open the site https://whois.domaintools.com and perform a search. We can see the resolved hostname below.
</p>
<br />


<p>
<img width="542" alt="Screenshot 2024-06-07 at 7 03 20 PM" src="https://github.com/RMBaez/Artifact-Extraction/assets/170957530/606c2bee-b9d7-4937-96b3-ac3985c8855e">
</p>

<p>
Question 7. The easiest way to retrieve this artifact is to right-click the hyperlink when viewing the file in an email client, and select ‘Copy Hyperlink’ (or a similar option).
</p>
<br />


<p>
<img width="546" alt="Screenshot 2024-06-07 at 7 07 02 PM" src="https://github.com/RMBaez/Artifact-Extraction/assets/170957530/1853f4e9-0aa3-4e26-8c31-b7108f382bd7">
</p>

<p>
Question 8. To find this we can either right-click the link in the email and select ‘copy link location’ and paste it into a program such as Notepad to see the URL text, or search for ‘http’ or ‘https’ in the email file until we find the right link. The ‘root domain’ essentially means the domain name of the URL, not including the specific resource. The root domain is ‘thiswouldbeamalicioussite.com’.
</p>
<br />
