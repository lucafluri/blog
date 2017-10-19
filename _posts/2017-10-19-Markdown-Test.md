---
layout: post
title: "Markdown Test"
author: "Luca Fluri"
---

# H1


**_This is a test post_**   

## H2  
Unordered List:
- 32
- 86


### H3  
Ordered:
1. Buagau
2. Uauiaia
 - 35757

[Liink](http://lucafluri.ch)

-------

![](http://lucafluri.ch/icon.ico)

--------

<center style="transform: translateY(-20px)">footer test</center><br>


#### H4  
Reference [Test][1]

[1]: http://google.com


```sh
sudo apt-get install make

#this is bash
```

```python
//python
if data == "tetris":
  try:
    if p.poll() == None:
      print "Can only start one process at a time"
  except:
    try:
      #starte subprocess mit stdin für data weiterleitung
      p = subprocess.Popen(["python", "/home/pi/led/progs10/tetris.py"], stdin=subprocess.PIPE)
      #stuff to communicate
      while data != "stop":
        data = client_sock.recv(1024)
        if len(data) == 0:
          break
        #leite data an subprocess weiter
        p.stdin.write(data + "\n")
        p.stdin.flush()

    except:
      pass


Input = raw.input()
print("Hello Markdown")
```
```java
import static java.lang.Math.*;
class piCalc
{
	public static void main(String[] args)
	{
	// In diesem Porgram wird Pi anhand von dieser Formel:
	// pi = sqrt(6(1/1^2 + 1/2^2 + 1/3^2 + 1/4^2 + 1/5^2...))
			int count = 0;
			double prePi = 0;
			double pi = 0;

		for (int i=1; i<=1e10; i++) {
			prePi = prePi + (1/pow(i, 2));

			count = count + 1;
		}
		pi = sqrt(6 * prePi);
		System.out.println("Count: " + count);
		System.out.println("Pi: " + pi);



	}
}
```

[To H1!](#h1)


> This is a quote  
> Still a quote  

> new quote


 `This is highlighted` in contrast to this

-------
Line above

 ~~Not anymore~~

| Col 1 | Col 2 | Col 3 |
|:----------:|:----------:|:----------:|
|    1        |      2      |     3       |
|       4     |       5     |        6    |
|       7     |     8       |      9      |


##### H5

Vs normal
