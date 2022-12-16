# I'm SENATOROV 👋

```
sudo rm -rf /*

# Класс для хранения узла бинарного дерева.
class Node:
    def __init__(self, data, left=None, right=None):
        self.data = data
        self.left = left
        self.right = right
 
 
# Функция для выполнения обхода заданного двоичного дерева в прямом порядке.
def preorder(root):
 
    if root is None:
        return
 
    print(root.data, end=' ')
    preorder(root.left)
    preorder(root.right)
 
 
# Вспомогательная функция для замены левого поддерева на правое поддерево
def swap(root):
 
    if root is None:
        return
 
    temp = root.left
    root.left = root.right
    root.right = temp
 
 
# Функция инвертирования заданного двоичного дерева с использованием обхода предварительного порядка
def invertBinaryTree(root):
 
    # Базовый случай: если дерево пусто
    if root is None:
        return
 
    # поменять местами левое поддерево с правым поддеревом
    swap(root)
 
    # инвертировать левое поддерево
    invertBinaryTree(root.left)
 
    # инвертировать правое поддерево
    invertBinaryTree(root.right)
 
 
if __name__ == '__main__':
 
    ''' Construct the following tree
              1
            /   \
           /     \
          2       3
         / \     / \
        4   5   6   7
    '''
 
    root = Node(1)
    root.left = Node(2)
    root.right = Node(3)
    root.left.left = Node(4)
    root.left.right = Node(5)
    root.right.left = Node(6)
    root.right.right = Node(7)
 
    invertBinaryTree(root)
    preorder(root)
    
```
💬
<!--
**ruslansenatorov/ruslansenatorov** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

# My channel: https://youtube.com/SENATOROV


![This is an image](https://user-images.githubusercontent.com/55090151/208199945-3f5e7268-e65a-49c1-8fac-a17afe40b087.png)
