# Task Planner

This project is web/mobile application which helps the user to track multi-step tasks in a convenient and smart way.

App gets the input for a task from the user and splits it up to sub steps with the help of LLMs trained for "task-splitting".
* User creates a new task
* writes or dictates the app the task definition and desired duration
* LLM asks for detail if needed and splits the task into sub steps and prioritizes and schedules each step.
* app displays the substeps in a github timeline format, according to the tasks duration.
  * for intra day tasks each dot represents the hour
  * for intra week tasks each dot represents days,
  * etc
* Non started dots will be represented as gray, started tasks will be blue, delayed/late tasks orange and completed tasks as green
* A reminder may assist user about the starting tasks
* When user reschedules a task, then the following tasks will be posponed accordingly
* Each sub step may have different owners with different roles, a simple RACI format may be filled optionally
  * Status change notification will be delivered to the role owners
  * Each RACI role may have different notification rules 
* Each sub step may have different attributes
  * Every action in relation with the sub step can be documented in a different formats
  * For example, any number of "Meeting Action"s may be added to the sub step
  * Or, any number of "Literature Review" attribute may be added the each sub step
  * Each attribute has its own format for input with optional and mandatory fields.
* Tasks may be a part of project or a program if indicated.
  * seperate tasks may be aggregated under a project later with "make project from task" functionality
  * or related tasks can be selected under "create project" function.
