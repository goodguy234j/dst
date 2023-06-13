# dst
class Node:
    def __init__(self,data):
        self.data=data
        self.ref=None
        self.pref=None


class doublellist:
    def __init__(self):
        self.head=None
        
    def print_LL(self):
        if self.head == None:
            print("linkedlist is empty")
            
        else:
            n=self.head
            while n is not None:
                print(n.data,"-->",end=" ")
                n= n.ref

    def when_e(self,data):
        new_node=Node(data)
        if self.head is None:
            self.head=new_node
            
    def add_b(self,data):
        new_data= Node(data)
        new_data.ref=self.head
        self.head.pref=new_data
        self.head=new_data

                
    def reverse_l(self):
        if self.head == None:
            print("linkedlist is empty")
            
        else:
            n=self.head
            while n.ref is not None:
