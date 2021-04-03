# TOOLAPIS

```tool:ReadAllText(string:filepath)```

 - Read all the contents of the file and return

```tool:WriteAllText(string:filepath,string:texts)```

 - Overwrite file writing
 - When the file does not exist, it will be created automatically

```tool:AppendAllText(string:filepath,string:texts)```

 - Append to the file
 - When the file does not exist, it will be created automatically

```tool:IfFile(string:filepath)```

 - Return a bool value to determine whether the file exists

```tool:IfDir(string:dirpath)```

 - Return a bool value to determine whether the folder exists

```tool:CreateDir(string:dirpath)```

 - Create a folder
 - Note: Multi-level folders cannot be created

```tool:HttpGet(string:url)```

 - Initiate a remote HttpGet request
 - Note: This method is not asynchronous

```tool:Schedule(function:func,int:delay,int:cycle)```

 - Set a timer
 - delay: execution interval, in milliseconds
 - cycle: number of executions
 - Return a task id of int type, which can be used to abort the task

```tool:Cancel(int:id)```

 - Abort a task with task id
 - Return a bool for success

```tool:TaskRun(function:func)```

 - Execute a function asynchronously

```tool:ToInt(object:number)```

 - Convert number to unsigned integer

```tool:NewGuid()```

 - Return a Guid