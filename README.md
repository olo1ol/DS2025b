3/31
링크드 리스트 노드, 포인터, 헤드, 마지막은 none
이중 링크드 리스트(양방향), 환형 링크드 리스트(순환)
class Node:
def __init__(self, data, link=None):
  self.data = data
  self.link = link

class LinkedList:
  def __init__(self):
    self.head = None

  def append(self, data):
    if not sefl.head:        #링크드 리스트의 노드가 하나도 없으면
      self.head = Node(data)  #새 노드를 head에 연결
      return
    current = self.head
    while current.next:
      currentt = current.next  #다음으로 이동
    current.next = Node(data)

ll = LinkedList()
ll.append(8)
