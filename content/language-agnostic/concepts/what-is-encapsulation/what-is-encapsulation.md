---
Title: "What is a Encapsulation?"
Subjects:
  - "Computer Science"
  - "Web Development"
Tags:
  - "Best Practices"
  - "Memory"
Catalog Content:
  - "https://www.codecademy.com/learn/paths/code-foundations"
  - "https://www.codecademy.com/learn/paths/computer-science"
  - "https://www.codecademy.com/learn/paths/web-development"
---

Encapsulation is one of the four principles of programming which emphasize modularity and hiding away of complexities in order to better maintain and reason about code. 

Most of the time encapsulation can be achieved by creating classes and naming private and public methods (or getters and setters) for our systems to interact.  
 
## Examples of Encapsulation

```py
class Robot(object):
   def __init__(self):
      self.__version = 22

   def getVersion(self):
      print(self.__version)

   def setVersion(self, version):
      self.__version = version

obj = Robot()
obj.getVersion()
obj.setVersion(23)
obj.getVersion()
print(obj.__version)
```