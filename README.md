# Signal
## 2018 Hanium Contest submissions
## Project Name: Authentication method used sonic waves
## Warn) Only Andriod Application Part (if you want to use this system, you must build DB, Web Server and PHP page)
## Communication) Use HTTP Communication

## Function
1. Join membership
2. Log in
3. Authentication apply Diffie-Hellman
4. Authentication use set password

## Authentication apply Diffie-Hellman
1. (Create P key when joining a member
2. Create Q key on login
3. Create an app's private key and public key using the authentication button
> 1. app`s Private Key: a, Sever`s Private Key: b
> 2. application Public Key:  A = q^a mod p, Server Public Key: B = q^b mod p
4. Exchange each of the public keys and forward the message to the plain.
5. Encrypt messages for authentication with private and public keys
> 1. massage: m
> 2. encryption massage: en_msg = m*A
6. Send encrypted messages to frequencies that come through a grid
7. Device that recognizes the transmitted frequency replaces the frequency value with the value from the table and sends it to the server
8. Compare the values passed to the server with the values that the server has
> M*B^a mod p = M*A^b mod p
> (Servers know A, B, p, and M.)
9. Successful authentication if matched

## 2018 한이음 공모전 출품작
## 프로젝트 명: 음파를 이용한 인증수단 개발
## 주의) 어플리케이션 부분만 있습니다.(DB제작, 웹 페이지 제작 필요)
## 통신) Http 통신을 사용합니다.
## 기능
1. 회원 가입
2. 로그인
3. 디피-헬만을 응용한 인증
4. 설정한 비밀번호를 사용한 인증

## 디피-헬만을 이용한 인증
1. 회원가입시 p키 생성
2. 로그인 시 q키 생성
3. 인증버튼을 통해 p, q를 이용해서 어플의 개인키, 공개키를 생성
> 1. 어플리케이션 개인키: a, 서버의 개인키: b
> 2. 어플리케이션 공개키: A = q^a mod p, 서버의 공개키: B = q^b mod p
4. 각각의 공개키를 교환 및 메시지를 평문으로 전달
5. 개인키와 공개키를 통해 인증에 사용할 메시지를 암호화
> 1. 메시지 m
> 2. 암호화된 메시지 en_msg = m*A
6. 암호화된 메시지를 대차표를 통해 나오는 주파수로 송출
7. 송출된 주파수를 인식한 단말기가 주파수 값을 대차표를 통해 나온 값으로 치환 후 서버에 전송
8. 서버에 전달된 값을 서버가 가지고 있는 값을 가지고 만든 값과 비교
> M*B^a mod p = M*A^b mod p
> (서버는 A, b, p, M을 알고있다.)
9. 일치하면 인증성공

