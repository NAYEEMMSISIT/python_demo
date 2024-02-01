class ToDoList:
    def __init__(self):
        self.tasks = []

    def add_task(self, task):
        self.tasks.append(task)

    def view_tasks(self):
        print("Tasks:")
        for task in self.tasks:
            print(f"- {task}")

    def remove_task(self, task):
        if task in self.tasks:
            self.tasks.remove(task)
            print(f"Task '{task}' removed.")
        else:
            print(f"Task '{task}' not found.")

my_todo_list = ToDoList()
my_todo_list.add_task("Finish Python project")
my_todo_list.add_task("Study for exams")
my_todo_list.view_tasks()
my_todo_list.remove_task("Study for exams")
