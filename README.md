# Assessment
@@ -71,10 +71,11 @@ body {
	position: absolute;
	top: -155px;
	width: 100%;
	padding: 50px;
	font-size: 100px;
	font-weight: 100;
	text-align: center;
	color: rgba(175, 47, 47, 0.15);
	color: #555555;
	-webkit-text-rendering: optimizeLegibility;
	-moz-text-rendering: optimizeLegibility;
	text-rendering: optimizeLegibility;
@@ -85,13 +86,13 @@ body {
	position: relative;
	margin: 0;
	width: 100%;
	font-size: 24px;
	font-family: inherit;
	font-size: 25px;
	font: Roboto;
	font-weight: inherit;
	line-height: 1.4em;
	border: 0;
	color: inherit;
	padding: 6px;
	color: #808080;
	padding: 25px;
	border: 1px solid #999;
	box-shadow: inset 0 -1px 5px 0 rgba(0, 0, 0, 0.2);
	box-sizing: border-box;
@@ -100,7 +101,7 @@ body {
}

.new-todo {
	padding: 16px 16px 16px 60px;
	padding: 24px;
	border: none;
	background: rgba(0, 0, 0, 0.003);
	box-shadow: inset 0 -2px 1px rgba(0,0,0,0.03);
@@ -115,6 +116,7 @@ body {
.toggle-all {
	width: 1px;
	height: 1px;
	padding: 24px;
	border: none; /* Mobile Safari */
	opacity: 0;
	position: absolute;
@@ -125,6 +127,7 @@ body {
.toggle-all + label {
	width: 60px;
	height: 34px;
	padding: 24px;
	font-size: 0;
	position: absolute;
	top: -52px;
@@ -135,13 +138,13 @@ body {

.toggle-all + label:before {
	content: '❯';
	font-size: 22px;
	color: #e6e6e6;
	padding: 10px 27px 10px 27px;
	font-size: 25px;
	color: #808080;
	padding: 24px;
}

.toggle-all:checked + label:before {
	color: #737373;
	color: #555555;
}

.todo-list {
@@ -152,7 +155,9 @@ body {

.todo-list li {
	position: relative;
	font-size: 24px;
	font-size: 25px;
	padding: 24px;
        color: #555555;
	border-bottom: 1px solid #ededed;
}

@@ -168,7 +173,7 @@ body {
.todo-list li.editing .edit {
	display: block;
	width: 506px;
	padding: 12px 16px;
	padding: 24px;
	margin: 0 0 0 43px;
}

@@ -202,23 +207,32 @@ body {
	background-image: url('data:image/svg+xml;utf8,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20width%3D%2240%22%20height%3D%2240%22%20viewBox%3D%22-10%20-18%20100%20135%22%3E%3Ccircle%20cx%3D%2250%22%20cy%3D%2250%22%20r%3D%2250%22%20fill%3D%22none%22%20stroke%3D%22%23ededed%22%20stroke-width%3D%223%22/%3E%3C/svg%3E');
	background-repeat: no-repeat;
	background-position: center left;
	font: awesome–fa-circle;
        font-size: 25px;
	padding: 24px;
        color: #555555;
}

.todo-list li .toggle:checked + label {
	background-image: url('data:image/svg+xml;utf8,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20width%3D%2240%22%20height%3D%2240%22%20viewBox%3D%22-10%20-18%20100%20135%22%3E%3Ccircle%20cx%3D%2250%22%20cy%3D%2250%22%20r%3D%2250%22%20fill%3D%22none%22%20stroke%3D%22%23bddad5%22%20stroke-width%3D%223%22/%3E%3Cpath%20fill%3D%22%235dc2af%22%20d%3D%22M72%2025L42%2071%2027%2056l-4%204%2020%2020%2034-52z%22/%3E%3C/svg%3E');
        font: awesome–fa-circle;
        font-size: 25px;
	padding: 24px;
        color: #555555;

}

.todo-list li label {
	word-break: break-all;
	padding: 15px 15px 15px 60px;
	padding: 24px;
	display: block;
	line-height: 1.2;
	transition: color 0.4s;
}

.todo-list li.completed label {
	color: #d9d9d9;
	text-decoration: line-through;
	color: #555555;
	text-decoration: none;
}

.todo-list li .destroy {
@@ -280,6 +294,11 @@ body {
}

.todo-count {
	font: Roboto;
        font-size: 25px;
	padding: 24px;
        color: #555555;
        font-style: italic;
	float: left;
	text-align: left;
}
@@ -323,7 +342,7 @@ html .clear-completed:active {
	float: right;
	position: relative;
	line-height: 20px;
	text-decoration: none;
	text-decoration: underline;
	cursor: pointer;
}

