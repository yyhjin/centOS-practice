##  Maven 3.8 설치

1. 다운로드
```sh   
# wget --no-check-certificate https://dlcdn.apache.org/maven/maven-3/3.8.8/binaries/apache-maven-3.8.8-bin.tar.gz
```
2. 압축 풀기
```sh
# tar xvfz apache-maven-3.8.8-bin.tar.gz
```
3. 설치
```sh
# mv /root/apache-maven-3.8.8 /usr/local/poscodx2023/maven3.8
# ln -s /usr/local/poscodx2023/maven3.8 /usr/local/poscodx2023/maven
```

4. 설정(/etc/profile)
```sh
export PATH=$PATH:/usr/local/poscodx2023/maven/bin
```

5. 확인
```sh
# mvn --version
Apache Maven 3.8.8 (4c87b05d9aedce574290d1acc98575ed5eb6cd39)
Maven home: /usr/local/poscodx2023/maven
Java version: 17.0.8, vendor: Oracle Corporation, runtime: /usr/local/poscodx2023/java17
Default locale: ko_KR, platform encoding: UTF-8
OS name: "linux", version: "3.10.0-514.el7.x86_64", arch: "amd64", family: "unix"
``` 
