## git 2.9.5 설치

1. 의존성 라이브러리
```sh
# yum -y install curl-devel
# yum -y install expat-devel
# yum -y install gettext-devel
# yum -y install openssl-devel
# yum -y install zlib-devel
# yum -y install perl-devel
```

2. 다운로드
```sh
# wget --no-check-certificate https://mirrors.edge.kernel.org/pub/software/scm/git/git-2.9.5.tar.gz
```

3. 압축 풀기
```sh
# tar xvfz git-2.9.5.tar.gz
```

4.소스 디렉토리 이동
```sh
  # cd git-2.9.5
```

5. configure compile & build Environment
```sh   
# ./configure --prefix=/usr/local/poscodx2023/git
```

6. 빌드
```sh
# make all
```
   
7. 설치
```sh   
# make install
```

8. old version 처리
```sh
# whereis git
git: /usr/bin/git /usr/share/man/man1/git.1.gz
# mv /usr/bin/git /usr/bin/git.old
# ln -s /usr/local/poscodx2023/git/bin/git /usr/bin/git
# git --version
git version 2.9.5
```
   
8. 설정(/etc/profile)
```sh
export PATH=$PATH:/usr/local/poscodx2023/git/bin
```

9. 확인
```sh   
# git --version
```

10. git 사용하기
```sh
# mkdir my-workspace
# cd my-workspace
# git clone https://github.com/yyhjin/java-study.git
# cd java-study
# mvn clean package
