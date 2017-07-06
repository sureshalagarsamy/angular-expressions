# AngularJS Expressions

AngularJS binds data to HTML using Expressions.

* AngularJS expressions can be written inside double braces: ```{{ expression }}```.
* AngularJS expressions can also be written inside a directive: ```ng-bind="expression"```.

### sample code

```html
<!DOCTYPE html>
<html>
<head>
	<meta charset="UTF-8">
	<title>AngularJS sample application</title>
	<link rel="shortcut icon" href="images/icon.png" />
	<link rel="stylesheet" href="css/styles.css">
	
	<script src="js/angular-1.5.4.js"></script>
</head>

<body ng-app>
	<p>#1 expression : {{ 5 + 5 }}</p>
	<p ng-init="quantity=3; cost=6">#2 expression : {{ quantity * cost }}</p>
	<p ng-init="firstName='Suresh';lastName='Alagarsamy'">#3 expression : {{ firstName + " " + lastName }}</p>
	<p ng-init="company='Abc'; location='Bengaluru'">#4 expression : <span ng-bind="company + ' ' + location"></span></p>
	<p ng-init="person={firstName:'Suresh',lastName:'Alagarsamy'}">#5 expression : {{ person.lastName }}</p>
</body>

</html>
```

### output 

![image](https://user-images.githubusercontent.com/6780840/27905749-935d9354-625e-11e7-8453-9ba680cedaae.png)
