mule-dbsaas-rest-project
========================

## URLs for various HTTP Operations:

```console
Base_Url: http://localhost:8081/api
insert POST <Base_Url>/emp  Creates a employee resource using the data included in the request.
get GET <Base_Url>/emp/<id> Returns the specified employee resource.
update PUT <Base_Url>/emp/<id>  Updates the specified employee resource.
delete DELETE <Base_Url>/emp/<id>  Deletes the specified employee resource.
```

### GET - To retrieve Employee by Id
http://localhost:8081/api/emp/<empId>

### GET - To retrieve all Employees list
http://localhost:8081/api/emp/all


### POST - To create Employee 

http://localhost:8081/api/emp
* HTTP Headers: Content-Type: application/json
* Sample JSON Payload:
```console
{
    "employeeId":"901",
    "firstName":"Jane",
    "lastName": "Miller",
    "hireDate": null,
    "email": "jane.miller",
    "departmentName":"Sales"
}
```

### DELETE - To delete Employee 

http://localhost:8081/api/emp/<empId>

### PUT- To update Employee 

http://localhost:8081/api/emp/<empId>
* HTTP Headers: Content-Type: application/json


## Compiling

### Build & Compile:
```console
$mvn clean compile package
```

