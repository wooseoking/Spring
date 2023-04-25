- JUnit

  - 단위 테스트 APi
  - Spring JUnit에서 사용하는 Annotation

-----------------------
1.@ RunWith(SpringJunit4ClassRunner.class)
  -  ApplicationContext를 만들고 관리할 수 있도록 JUnit 기능을 확장시킨다. <br>
  -> 원래 JUnit 에서는 테스트 메서드별로 객체를 따로 생성해서 관리하지만 Spring-test 라이브러리로 확장된 JUnit은 컨테이너 기술을 이용해서 싱글토으로 객체를 관리한다.
  
  
  
2.@ContextConfiguration(locations = "classpath:xml경로")
- Bean configuration에 대한 경로 설정

3.@Test
- 단위 테스트할 메서드에 선언

4.Ignore
- 테스트 실행하지 않도록 지정

5.@ BeforeClass/ @AfterClass
- 클래스에서 한번만 수행되는 메서드

6.@ Before / @After
- 모든 테스트 메서드가 수행되기전, 후로 실행되는 메소드 지정<br>
-> 공통으로 실행되어야 하는 기능을 지정한다.
-----------------------------

■ assert(단정) 메서드 
assertEquals(x,y) 	: 두 객체가 일치하는 검사<br>
assertFalse(x)	: 값이 false인지 확인 <br>
assertTrue(x)	: 값이 true인지 확인 <br>
assertNull(x)	: 값이 null인지 확인 <br>
assertNotNull(x)	: 값이 null이 아닌지 확인 
