# Using-tools-like-John-the-Ripper-for-password-cracking
## AIM:
To crack password hashes using John the Ripper in Kali Linux.

## DESIGN STEPS:
### Step 1:
Install John the Ripper using the command

### Step 2:
Prepare the password hash file (e.g., using unshadow for Linux password and shadow files).


### Step 3:
Use John the Ripper to crack the hashes:

## PROGRAM:
Password Cracking with John the Ripper
- **Install the John Ripper**
  ```bash
  sudo apt install john
  ```
- **Create a Password-Protected ZIP File**
   Archive a normal file (secret.txt) into a password-protected ZIP file
   ```bash
   zip --password Anisha abc.zip abc
   ```
 - **Extract the Hash from the ZIP File**
   ```bash
   zip2john abc.zip > hash.txt
   ```
- **Crack the ZIP Password using John**
  ```bash
  john --format=zip hash.txt
  ```
- **Show the Cracked Password**
  ```bash
  john --show hash.txt
  ```
  
1.Creating a txt while and making it password protected. It will be stored in zip format.
![WhatsApp Image 2025-04-26 at 10 56 47_4f98d2af](https://github.com/user-attachments/assets/99261937-ab10-431e-b5dd-9458bc6b7426)
![image](https://github.com/user-attachments/assets/20e345d6-d529-4efe-97a3-58764bbc4406)
![WhatsApp Image 2025-04-26 at 10 57 51_aa919313](https://github.com/user-attachments/assets/178e5d2a-c9f9-4a8a-a212-85a7806b7df7)

2. Using John the Ripper make sure the zip file exists
![WhatsApp Image 2025-04-26 at 10 58 08_b17b935d](https://github.com/user-attachments/assets/2304c91d-edb9-40a7-b6ae-1a43dd4ac0e1)
![WhatsApp Image 2025-04-26 at 11 00 57_b3949407](https://github.com/user-attachments/assets/8bda9566-dd81-4cf5-8e22-2a10decb018d)

3. Generate Hash using zip2john and verify
![WhatsApp Image 2025-04-26 at 11 02 28_f4dac5f2](https://github.com/user-attachments/assets/dd9e761e-c473-448a-97e7-55db79f8121e)

4.Start cracking the password and view it
![image](https://github.com/user-attachments/assets/cb7b6387-fc1e-49bc-96c8-4ae33d41bc34)


## OUTPUT:
The terminal will display the filename and its cracked password.
![image](https://github.com/user-attachments/assets/07f7cc84-52fe-446b-8b8e-89e617dd4ed8)


## RESULT:
The password hashes were successfully cracked using John the Ripper.

