# SpringBoot에서 SpringSecurity 적용하기 

SpringBoot에서 인증,권한, 보안처리를 위해 SpringSecurity를 적용하는 방법을 알아 보겠습니다. 먼저 의존성을 추가합니다. 

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-security</artifactId>
</dependency>
```
자바 Configuration 파일을 만들고 @EnableWebSecurity, @Configuration 어노테이션을 추가합니다. 

```java
@EnableWebSecurity
@Configuration
public class WebSecurityConfig extends WebSecurityConfigurerAdapter {
}
```

@EnableWebSecurity 어노테이션은 SpringSecurity를 활성화 시키는 어노테이션입니다. 이 어노테이션을 추가하면 SpringSecurity가 활성화 되고 기본적인 보안설정이 적용됩니다. 이 어노테이션은 자동 설정하는 클래스들이 매우 많은데, 지금은 자동설정(autoconfiguration)을 해준다고만 알고 있으면 됩니다. 



























