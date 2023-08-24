java17 설치
JDK 다운로드
# wget https://download.oracle.com/java/17/archive/jdk-17.0.8_linux-x64_bin.tar.gz
압축을 푼다
# tar xvfz jdk-17.0.8_linux-x64_bin.tar.gz 
poscodx2023 소프트웨어 설치 디렉토리 만들기
# mkdir /usr/local/poscodx2023
설치
# mv /root/jdk-17.0.8 /usr/local/poscodx2023/java17
링크 파일 생성
# ln -s /usr/local/poscodx2023/java17 /usr/local/poscodx2023/java
설정(/etc/profile)
export JAVA_HOME=/usr/local/poscodx2023/java
export CLASSPATH=$JAVA_HOME/lib/*
export PATH=$PATH:$JAVA_HOME/bin
현재 shell 환경에 적용하기
# source /etc/profile
확인
# java --version
java 17.0.8 2023-07-18 LTS
Java(TM) SE Runtime Environment (build 17.0.8+9-LTS-211)
Java HotSpot(TM) 64-Bit Server VM (build 17.0.8+9-LTS-211, mixed mode, sharing)
