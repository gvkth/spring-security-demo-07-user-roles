# spring-security-demo-07-user-roles
Phải thêm vào pom.xml thư viện spring-security-taglibs
<!-- Add Spring Security Taglibs support-->
		<dependency>
			<groupId>org.springframework.security</groupId>
			<artifactId>spring-security-taglibs</artifactId>
			<version>${springsecurity.version}</version>
		</dependency>


  #Sử dụng trong jsp files:

    Đầu file thêm khai báo sử dụng taglib:
      <%@ taglib prefix="security" uri="http://www.springframework.org/security/tags"  %>
    Trong file, sử dụng
      <security:authentication property="principal.username" />

      <span><security:authentication property="principal.authorities" />
