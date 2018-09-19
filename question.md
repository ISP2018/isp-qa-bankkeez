#Questions

**Q1.** As a beginner developer, you are new to a lot of things, you have a chance to ask an expert a question. You asked him how to become a good developer like you. He answered, **"Don't reinvent the wheel when you can steal it".** What do you think an expert mean according to the choices: 
**(Choose all choices if they are all correct)**

(One of correct choice): As a beginner developer, you'll find the problem that that you're trying to solve that has already been solved by somebody else. Design patterns are generic solution. So as framework that extends those pattern for simplifying your application.

Reference: [https://softwareengineering.stackexchange.com/questions/34173/are-there-concrete-reasons-not-to-use-libraries-and-code-snippets-heavily]

**Q2.** 
``` @Test
public void testDivide(){
double x = 5;
double y = 30000;
assertEquals(0.00016,5/30000);
}
```
Is the code correct or it is wrong? If wrong then fix the code.

Answer: 
``` 
static final double TOL = 1.0E-5;
@Test
public void testDivide(){
double x = 5;
double y = 30000;
double expected = 0.00016666666666666;
assertEquals(expected,5/30000,TOL);
}
```




