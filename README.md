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


<p>
<img width="541" alt="image" src="https://github.com/RMBaez/Artifact-Extraction/assets/170957530/d3372b6e-a5fd-4ff9-a7ea-1d6f8eab9e7e">
</p>

<p>
Question 9. Same as before, we'll use Find and search for “From”.
</p>
<br />


<p>
<img width="541" alt="image" src="https://github.com/RMBaez/Artifact-Extraction/assets/170957530/4130de1d-f8d1-4989-8b95-55cd9459fd55">
</p>

<p>
Question 10. Searching for the “To” field and value.
</p>
<br />


<p>
<img width="541" alt="Screenshot 2024-06-07 at 7 16 25 PM" src="https://github.com/RMBaez/Artifact-Extraction/assets/170957530/81a51ff1-c4b0-4762-a267-57f33f238483">
</p>

<p>
Questoin 11. Searching for the “To” field and value.
</p>
<br />


<p>
<img width="541" alt="image" src="https://github.com/RMBaez/Artifact-Extraction/assets/170957530/eb374b24-2a0d-4522-83ec-b3ac31964d1b">
</p>
  
<p>
Question 12. Searching for the “Date” field and value.
</p>
<br />


<p>
<img width="334" alt="image" src="https://github.com/RMBaez/Artifact-Extraction/assets/170957530/a2c5d7fa-ed1c-4ae6-bd99-bb7fc8bd3b35">
</p>

<p>
Question 13. We'll search for the “X-Sender-IP” field and its value.
</p>
<br />


<p>
<img width="594" alt="image" src="https://github.com/RMBaez/Artifact-Extraction/assets/170957530/b02f5162-9866-431d-a731-0227cd9dc002">
</p>

<p>
Question 14. Using the IP from the previous question, we'll submit it to https://whois.domaintools.com.
</p>
<br />


<p>
<img width="545" alt="image" src="https://github.com/RMBaez/Artifact-Extraction/assets/170957530/480d7f9d-265c-4009-b913-894eacfefbe4">
</p>

<p>
Question 15. From within the text editor we can search for “filename”.
</p>
<br />

<p>
<img width="545" alt="image" src="https://github.com/RMBaez/Artifact-Extraction/assets/170957530/be2871cc-c8d6-41fa-9203-d2d422920b35">
</p>

<p>
Question 16. In Thunderbird we can right-click the attachment and click Save-As, then save it to the Desktop. We'll then open a PowerShell window and use the Get-FileHash cmdlet to retrieve the MD5 and SHA256 hashes. As SHA256 is the default hashing algorithm we don't need to state it, however we must do this for MD5.
</p>
<br />
