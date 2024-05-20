#### General
Checks if we are who we say we are.
	- often in "form based" --> login portal

#### Vulnerable
Arise from insecure implementation of the authentication mechanisms in an application.


## Example Types
1. Weak Password Requirements:
![[Pasted image 20240513222910.png]]
- if using off-the-shelf software > check the online documentation for default passwords > try to use them
- NOTE: CASMM ( right legend in screenshot )

2. Improper Restriction of Authentication Attempts:
![[Pasted image 20240513223656.png]]

3. Verbose Error Message:
![[Pasted image 20240513223930.png]]
- error messages give you specific details: "username already exists"

4. Vulnerable Transmission of Credentials:
![[Pasted image 20240513224106.png]]

5. Insecure Forgot Password Functionality:
![[Pasted image 20240513224155.png]]


6. Defects in Multistage Login Mechanism
![[Pasted image 20240513224440.png]]
- business logic flaw


7. Insecure Storage of Credentials:
![[Pasted image 20240513224737.png]]
- Passwords should NOT be encrypted > they should be hashed


## Impact

#### CIA:
![[Pasted image 20240513225354.png]]

#### Risk:
![[Pasted image 20240513225317.png]]






# Resources:


Link:
https://academy.ranakhalil.com/courses/1491236/lectures/45273752


PART OF:
[[password_gtk]]


