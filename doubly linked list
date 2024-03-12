class Node:
  def __init__(self):
    self.data = 0 
    self.prev = None
    self.next = None
    
class DLinkedList:
    def __init__(self):
        self.head = None
        self.temp = None
        
    def append(self,num = 0):
      nn = Node()
      if num == 0:
        num = int(input("enter the new node value"))
        nn.data = num 
      else:
        nn.data = num 
        
      if self.head == None:
        #empty list
        self.head = nn
        self.temp = nn
      else:
        #list is present
        self.temp = self.head
        while(self.temp.next !=None):
          self.temp = self.temp.next
        self.temp.next = nn 
        nn.prev = self.temp
        
    def printList(self):                                                                
      print("list is")
      self.temp = self.head
      while(self.temp != None):
        print(self.temp.data,end = " ->")
        self.temp = self.temp.next
      print("none")
        
    def printBList(self):
      print("backward list is ")
      self.temp = self.head
      while(self.temp.next !=None):
          self.temp = self.temp.next
      while(self.temp != None):
          print(self.temp.data,end = "->")
          self.temp = self.temp.prev
      print("none")
          
if __name__ =="__main__":
  dLL = DLinkedList()
  dLL.append(10)
  dLL.append(20)
  dLL.append(30)
  dLL.printList()
  dLL.printBList()
