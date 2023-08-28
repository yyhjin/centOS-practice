## java17 설치

1. JDK 다운로드
```sh
# wget https://download.oracle.com/java/17/archive/jdk-17.0.8_linux-x64_bin.tar.gz
```  

2. 압축을 푼다
```sh
# tar xvfz jdk-17.0.8_linux-x64_bin.tar.gz 
```

3. poscodx2023 소프트웨어 설치 디렉토리 만들기
```sh
# mkdir /usr/local/poscodx2023
```

4. 설치
```sh
# mv /root/jdk-17.0.8 /usr/local/poscodx2023/java17
```

5. 링크 파일 생성
```sh
# ln -s /usr/local/poscodx2023/java17 /usr/local/poscodx2023/java
```

6. 설정(/etc/profile)
```sh
export JAVA_HOME=/usr/local/poscodx2023/java
export CLASSPATH=$JAVA_HOME/lib/*
export PATH=$PATH:$JAVA_HOME/bin
```

7. 현재 shell 환경에 적용하기
```sh
# source /etc/profile
```

8. 확인
```sh
# java --version
java 17.0.8 2023-07-18 LTS
Java(TM) SE Runtime Environment (build 17.0.8+9-LTS-211)
Java HotSpot(TM) 64-Bit Server VM (build 17.0.8+9-LTS-211, mixed mode, sharing)
```
