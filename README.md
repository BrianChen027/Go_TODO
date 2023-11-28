
# This the the TODO list using GO

This Go program is a to-do application designed to manage tasks, featuring functionalities like adding, completing, deleting, and listing to-dos. The program is split into two main files: **main.go** and **todo.go**.
         ![截圖 2023-11-28 上午2 14 34](https://github.com/BrianChen027/Go_TODO/assets/97871497/1c13252e-85f4-472a-94ed-6882ceacc9cb)

## main.go
### Features <br/>
    1. Flag Handling: Utilizes the flag package to parse command-line arguments. These flags include adding a new to-do (add), marking a to-do as completed (complete), deleting a to-do (del), and listing all to-dos (list).
    2. To-Do Operations: Performs different operations on to-dos, such as add, complete, delete, or list, based on the command-line arguments.
    3. Error Handling: If errors occur during operations, the program prints them to standard error output and exits. 
    4. User Input: If no to-do is directly specified for the add operation, the program reads the to-do item from standard input. 

### Process <br/>
    1. Parses command-line arguments. 
    2. Loads the to-do file. 
    3. Executes the corresponding to-do operation based on the command-line arguments. 
    4. Handles user input. 
    5. Saves changes to the to-do file.

## todo.go <br/>

### Features <br/>
    1. To-Do Management: Provides a Todos structure to manage a list of to-do items. 
    2. CRUD Operations: Adds new to-dos, marks them as completed, deletes to-dos, and lists all to-dos. 
    3. Persistence: Saves to-do list to a file and loads from it. 
    4. Formatted Output: Uses the simpletable package for formatted output of the to-do list.

### Process <br/>
    1. Adds, marks as complete, and deletes to-do items. 
    2. Loads and saves to-do data to/from a file.
    3. Formats and outputs the list of to-dos. 


## This is how the TODO table shows
<img width="816" alt="截圖 2023-11-24 下午4 02 09" src="https://github.com/BrianChen027/Go_TODO/assets/97871497/1c4f7805-614e-4c4d-a334-d92c05299797">

## Once the task is completed, us "./todo -complete=2" to change the task's status to Done
<img width="815" alt="截圖 2023-11-24 下午4 07 59" src="https://github.com/BrianChen027/Go_TODO/assets/97871497/98b2f71c-cb02-4bfe-bd6e-227822410b09">

## If you want to add the task or delete the task, use "./todo -add "task1"" and "./todo -del=6" 
<img width="808" alt="截圖 2023-11-24 下午4 03 46" src="https://github.com/BrianChen027/Go_TODO/assets/97871497/cfedfe0a-7c72-4a1e-94ae-757d0c276671">

<br/>
<br/>
<br/>

#### ------------------------------------ The Tool reminder when using Go ------------------------------------


查看go目前版本 Check the current version of Go<br/>
go version <br/>
查看當前go的環境變數 View the current Go environment variables<br/>
go env <br/>
列出目前全部安裝的依賴函式庫 List all currently installed dependencies<br/>
go list <br/>
編輯並執行go程序 Edit and run a Go program<br/>
go run <br/>
自動更新依賴函式庫 Automatically update dependencies <br/>
go get -u <br/>
增加缺少的module， 刪除無用的module Add missing modules, remove unused modules<br/>
go mod tidy <br/>
建立mod檔案,它是管理依賴關係的一個檔案 create the go.mod for the project <br/>
go mod init github.com/BrianChen027/Go_TODO <br/>
go mod tidy <br/>
用於編譯 Go 程序 to build the project after modifing it, this can make sure it works <br/>
go build ./cmd/todo <br/>
