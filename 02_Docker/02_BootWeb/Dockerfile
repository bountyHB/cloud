FROM openjdk:11
LABEL maintainer ="kh<bounty@iei.or.kr"
LABEL version="1.0"
# /root 디렉터리에 05_SpringBoot_MVC-0.0.1-SNAPSHOT.jar 파일을 복사
COPY 05_SpringBoot_MVC-0.0.1-SNAPSHOT.jar /root
ENV TZ=Asia/Seoul
EXPOSE 8088
# 작업 디렉터리를 /root로 변경
WORKDIR /root
# 컨테이너 생성 시 05_SpringBoot_MVC-0.0.1-SNAPSHOT.jar 파일을 자동으로 실행하도록 명령
CMD ["java", "-jar", "05_SpringBoot_MVC-0.0.1-SNAPSHOT.jar", "--spring.profiles.active=dev"]