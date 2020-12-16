Tech Stack Used:
  Maven , H2 data base,Spring Boot , Spring  DATA and JPA ,Java8

Import the project as a simple maven project and run the application as spring boot application

End point details :

Below are end points urls and methods , please use POSTMAN app or SOAP UI to test api's
  Add Employee (id, firstName, lastName) 
    Method:POST 
    URL:http://localhost:8080/api/v1/employees 
      Request: { "id": 1, "firstName": "Test1", "lastName": "lastName1" }

  Edit Employee (firstName, lastName)
        Method:PUT 
        URL : http://localhost:8080/api/v1/employees/1 
        Request: { "id": 1, "firstName": "Test1", "lastName": "lastName1"}

  Delete Employee (id) 
    Method:Delete 
    URL:http://localhost:8080/api/v1/employees/1 
    Request : { "id": 1, "firstName": "Test1", "lastName": "lastName1"}
    Response: { "deleted": true }

  List of All Employees 
    Method:GET 
    URL:http://localhost:8080/api/v1/employees
    response: [{"id":1,"firstName":"Test1","lastName":"lastName1","emailId":"emailId1"},{"id":2,"firstName":"Test1","lastName":"lastName1","emailId":"emailId1"}]
  
  Get count of Employee present
    Method :GET
    URL : http://localhost:8080/api/v1/employeesCount
    Response : The count is : 1
