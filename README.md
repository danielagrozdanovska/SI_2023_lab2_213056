Daniela Grozdanovska 213056

2 чекор CFG: https://drive.google.com/file/d/1eP0NZQOowUih3wEcHRfYFaG2s2Munj3d/view?usp=sharing

3 чекор: Цикломатската комплексност е 11. Ја пресметав така што ги изброив предикатните јазли и додадов 1.

4 чекор: https://docs.google.com/spreadsheets/d/1qSf8XCSzgPvNiCVj7pNP63LC-DLZaOWC/edit?usp=sharing&ouid=109388851760592006232&rtpof=true&sd=true
1. null

2. username null
email contains @ and . 
pwLength<8 
existing user and existing email
username: null	
password: dani12 (lenght=6)	
email: daniela@gmail.com

3. username not null, 
email do not contain @ and . 
password do not contains username and its length is not less than 8
password do not conatins " "
password contains special character 
username: daniela	
password: finkiukim1$	
email: danielagmailcom

4. password does not contain special character
not existing user
username daniela
password finkiukim
email: daniela@gmail.com


5 чекор:
T	X	X	  T 	user=null;      password=dani123!;   email=dani@gmail.com
F	T	X	  T 	user=daniela;   password= null;      email=dani@gmail.com
F	F	T	  T	  user=daniela;   password=dani123!;   email=null
F	F	F 	F 	user=daniela;   password=dani123!;   email=dani@gmail.com
Кога имаме OR со 3 променливи, првите 4 реда ги групираме во T X X -> бидејќи првата променлива има вредност Т, не е важно која е вредноста на другите 2 променливи -> ќе врати Т, наредните 2 реда F T X -> бидејќи првата променлива има вредност F, ја проверуваме втората - бидејќи втората има вредност Т, немаме потреба да ја проверуваме третата -> ќе врати Т, наредниот еден ред F F T бидејќи и првата и втората променлива се F, ја проверуваме и третата и бидејќи таа е Т -> враќа Т, и последниот ред каде сите се F F F -> враќа F




