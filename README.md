<!DOCTYPE html>
<html>
<head>
  <title>My Data</title>
</head>
<body>
  <h1>My Data</h1>
  <ul>
    <li><strong>Name:</strong> John Doe</li>
    <li><strong>Age:</strong> 30</li>
    <li><strong>City:</strong> New York</li>
  </ul>
   <script>
    var myData = [
      {name: "John Doe", age: 30, city: "New York"},
      {name: "Jane Doe", age: 25, city: "Los Angeles"},
      {name: "Bob Smith", age: 40, city: "Chicago"}
    ];
    var table=document.createElement("table");
    table.border = 1;
    var tr = table.insertRow(0);
    var th1 = tr.insertCell(0);
    var th2 = tr.insertCell(1);
    var th3 = tr.insertCell(2);
    th1.innerHTML = "Name";
    th2.innerHTML = "Age";
    th3.innerHTML = "City";
     for (var i =0;i<myData.length; i++) {
      var tr = table.insertRow(i+1);
      var td1 = tr.insertCell(0);
      var td2 = tr.insertCell(1);
      var td3 = tr.insertCell(2);
      td1.innerHTML =myData[i].name;
      td2.innerHTML = myData[i].age;
      td3.innerHTML =myData[i].city;
    }    document.body.appendChild(table);
  </script>
</body>
</html>
