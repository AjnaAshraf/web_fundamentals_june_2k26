### API 
---
```Application programming interface that enables communication bw different applications```


### Webfundamentals
---

## client server architeture
    ```client sends an http request to server, server process the http request and send back http response ```

### http_methods
---
`GET` => fetch all resources  
`POST` => create an new resource  
`PUT` => update a resource  
`PATCH` => UPDATE a resource (partial update)  
`DELETE` => delete a resource  


### http_request_format
---

`url`  
`http_method`  
`Authorization`  
`body`  

### sample api end point
---

```
Employee

id  name    age   department  salary

1   haris    23          hr      25000
2   vipin    23          qa      25000
3   jithn    23          it      25000
4   rahul    23          hr      25000

```

```
http_request for adding employee

url: localhost:8000/employee/
method:POST
body:{
    "name":"vysak",
    "age":24,
    "department":"hr",
    "salary":45000
}



```
---
```
http_request for listing employee

url:localhost:8000/employee/
method:GET

```

---
```
http_request for fetching specific employee detail

url : localhost:8000/employee/4/
method:GET

```

```
http_request for updating an employee 

url:localhost:8000/employee/4/
method:PUT
body:{
    "name":"Rahul",
    "age":24,
    "department":"hr",
    "salary":30000
}

```

```
http_request for deleting  specific employee 

url:localhost:8000/employee/4/
method:DELETE
```

### Movie task

```
Movie

id      title      year     language        run_time


1          kgf1      2008      kannada           160
2          kgf2      2020      kannada           165
3          kgf3      2026      kannada           167
4          kgf4      2028      kannada           168
5          kgf5      2030      kannada           169
```

`http_request for adding new movie`

```
url:localhost:8000/movie/
method:POST
body:{
"title":"BKU",
"year":2026,
"language":"malayalam",
"run_time":167
}

```
`http_request for list all movie`

```
url:localhost:8000/movie/
method:GET
```
`http_request for fetching movie detail`

```
url:localhost:8000/movie/4/
method:GET

```
`http_request for update movie`

```
url:localhost:8000/movie/4/
method:PUT
body:{
"title":"Athiradi",
"year":2026,
"language":"malayalam",
"run_time":160
}
```
`http_request for delete movie`

```
url:localhost:8000/movie/5/
method:DELETE

```

### HOSPITAL REGISTER MANAGEMENT TASK
---

```

hospital

id   patient_name  phone_no      assigned_doc      consultation_fee


1          Alia     9746756743      george          160
2          mick     8757389874      cam             200
3          aysha    7467393746      samuel          800
4          liam     9837647374      ron             450
5          daniel   8736541537      manu            180


```

` http request to add a patient register `

```

url:localhost:8000/hospital/
method:POST
body:{

    "patient_name":"Anjali",
    "phone_no":9367428777,
    "assigned_doc:"Hari",
    "consultation_fee":180

}

```
---

` http request to list all  patient registers `

```
url:localhost:8000/hospital/
method:GET
```

`http_request for fetching a petient register detail`

```
url:localhost:8000/hospital/3
method:GET

```

`http_request for update patient register`

```

url:localhost:8000/hospital/2
method:PUT
body:{

    "patient_name":"hiba",
    "phone_no":9367477345,
    "assigned_doc:"george",
    "consultation_fee":160

}

```


`http_request for delete a patient record`

```
url:localhost:8000/hospital/5/
method:DELETE

```
