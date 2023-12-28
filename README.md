# father_mother_child

# 定义第一个父类
class Father:
    def __init__(self):
        print("Father's constructor")
    
    def speak(self):
        print("Father speaks")

# 定义第二个父类
class Mother:
    def __init__(self):
        print("Mother's constructor")
    
    def listen(self):
        print("Mother listens")

# 定义子类，继承自Father和Mother
class Child(Father, Mother):
    def __init__(self):
        super().__init__()  # 调用父类的构造函数
        print("Child's constructor")

# 创建Child类的实例
child = Child()

# 调用继承自Father的方法
child.speak()

# 调用继承自Mother的方法
child.listen()
