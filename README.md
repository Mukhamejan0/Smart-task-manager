# Smart-task-manager
public class Main {
    public static void main(String[] args) {
        TaskManager taskManager = new TaskManager();

        User user = new User(1, "Mukhamedzhan", "mukha@email.com");

        Task task1 = new Task(
                "Finish OOP Project",
                "Prepare presentation and Java code",
                Priority.HIGH
        );

        Task task2 = new Task(
                "Upload to GitHub",
                "Push project files to repository",
                Priority.MEDIUM
        );

        taskManager.addTask(task1);
        taskManager.addTask(task2);

        taskManager.listTasks();
    }
}
