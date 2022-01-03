
<img style="float: right; width: 200px; height: 200px; border: 1px solid; margin-top: 5px;" src="assets/photo.jpg">

### Dmitriy Ivanov

#### Contacts:

- **tel. number:** +79518802381
- **e-mail:** ivanovdm812@gmail.com
- **github:** https:/github.com/wandel812
- **telegram:** @ivanovdm812
- **discord** 
    * *rs-school handle*: Ivanov Dmitriy (@wandel812)
    * *general handle*: pupsik812#8696


---

<br/>

## Summary:

A novice frontend-developer with technical education.

I like learning new things, having fresh experience and the feeling of overcoming difficulties. 

<br/>

## Skills:

**Programming languages and technologies:** JavaScript, HTML, CSS, Java, Python

**Tools:** GIT, VS Code, IntelliJ IDEA, pycharm, pyside, react, mui, chakraui

<br/>

## Code example: 

**Shortest Knight Path:** Given two different positions on a chess board, find the least number of moves it would take a knight to get from one to the other. The positions will be passed as two arguments in algebraic notation. For example, knight("a3", "b5") should return 1.

The knight is not allowed to move off the board. The board is 8x8.

```java
public class Chess {
    private static int[] dx = {1, -1, 1, -1,  2, 2, -2, -2};
    private static int[] dy = {2, 2, -2, -2, -1, 1,  1, -1};
    private static int moveOptionsCnt = 8;
    
    private static int depth = 24;
    private static int ans;
    private static boolean[][] used;
    
    private static void run(int sX, int sY, int fX, int fY, int stepsCnt) {    
      if (stepsCnt > ans || stepsCnt > depth)
        return;
        
      if (sX == fX && sY == fY) {
        if (ans > stepsCnt)
          ans = stepsCnt;
        return;
      }
      
      used[sX-1][sY-1] = true;
        
      for (int i = 0; i < moveOptionsCnt; i++) {
        int toX = sX + dx[i];
        int toY = sY + dy[i];
        if (0 < toX && toX < 9 && 0 < toY && toY < 9 && !used[toX-1][toY-1]) {
          run(toX, toY, fX, fY, stepsCnt + 1);
        }
      }
      
      used[sX-1][sY-1] = false;
      
    }
    
    public static int knight(String start, String  finish) {
        int sX = Integer.parseInt(start.substring(1,2));
        int sY = start.charAt(0) - 'a' + 1;
        int fX = Integer.parseInt(finish.substring(1,2));
        int fY = finish.charAt(0) - 'a' + 1;
        ans = 1000;
        used = new boolean[8][8];
        run(sX, sY, fX, fY, 0);
        
        return ans;
    }
}
```

<br/>

## Expirience:

1. During the practice period at university was an intern at the IT company "Neoflex". Programmed a parser for loan calculator 
website using Java.
1. Bachelor's degree graduation project -- "Automation of the construction of computational domains for the finite volume method"
was programmed using Python.
1. LANIT. 1.5 year. 
    - As QA wrote autotest using gherkin and selenide. 
    - Worked as developer on creation of an interface generator for training neural networks using python and qt framework. 
    - Developed one-page service work nn output displaying and convenient debugging using js, react, mui.

<br/>

## Education:

1. Saratov Chernyshevsky State University -- Applied Informatics.
1. QA school from LANIT company.
1. Introduction to Linux online course.

<br/>

## Languages: 

* Russian -- Native
* English -- B1
    - Language school for 3 years
    - An additional diploma of translator in professional area