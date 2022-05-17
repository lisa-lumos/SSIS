## SSIS Intro

Following the [YouTube link](https://www.youtube.com/watch?v=NGzieSedvuM&list=PL_YF--8vjjEVEXMf2hEFn0D5tEJV9kRqi): 


SQL Server Integeration Services (SSIS), useful for high performance ETL jobs (data migration). 

Have components for incremental load, lookup, join, CDC, SCD (includes code that is prewritten and tested). Compared with C#, can handle efficiently millions or billions of rows, even if machine run out of memory. Much less code to write. 

Could load file types such as flat files, excel files, xml files, etc. File source can be MySQL, Oracle, etc, without needing third party component. 

## Components of SSIS

Create a Integration Services Project in MS Visual Studio. 

View menu -> Solution Explorer

Control Flow window is where all SSIS tasks are situated. Create workflow here. 

Drag "Execute SQL Task" tool from SSIS Toolbox on the left. Connect different tools with dragging arrows. 

"Data Flow Task" tool is expecially designed for data migration. In "Data Flow", there are mainly 3 kinds of components: Source, transformation, destination. To write data to SQL Server, need to choose OLE DB Destination tool. 

You can use multiple Data Flow tasks in your Control Flow window. 

Parameter window: Can pass parameters to deployed packages (even outside of SSIS package, so SSIS package don't need to be modified). 

Event Handlers window: Could handle error. Shows error code, error description. 

Package Explorer window: See all system variables, etc. 

How is variables different from Parameters?

You can convert a package connection to project connection, the it will be available to all SSIS packages. 

dtsx file -> Data Transformation Services Package File

Output window: see error messages. 

Debug -> Windows -> Output window: get values at runtime. 

[mockaroo.com](mockaroo.com) can provide free data for testing purposes. 




