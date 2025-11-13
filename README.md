<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Library Management System</title>

<style>
    body {
        font-family: Arial, sans-serif;
        background: #f5f5f5;
        margin: 0;
        padding: 0;
    }

    .container {
        max-width: 1200px;
        margin: auto;
        padding: 20px;
    }

    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    nav button {
        padding: 8px 14px;
        background: white;
        border: 1px solid #ddd;
        border-radius: 6px;
        cursor: pointer;
        margin-left: 5px;
    }

    nav .active {
        background: #4f46e5;
        color: white;
    }

    .cards {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        gap: 15px;
        margin-top: 20px;
    }

    .card {
        background: white;
        padding: 20px;
        border-radius: 10px;
        box-shadow: 0px 2px 8px rgba(0,0,0,0.1);
    }

    .card-title {
        font-size: 14px;
        color: gray;
    }

    .card-number {
        font-size: 28px;
        font-weight: bold;
    }

    .section-title {
        margin-top: 30px;
        font-size: 20px;
        font-weight: bold;
    }

    table {
        width: 100%;
        margin-top: 15px;
        border-collapse: collapse;
        background: white;
        border-radius: 10px;
        overflow: hidden;
        box-shadow: 0px 2px 6px rgba(0,0,0,0.1);
    }

    th, td {
        text-align: left;
        padding: 12px 10px;
        border-bottom: 1px solid #eee;
    }

    th {
        background: #fafafa;
    }

    .actions a {
        margin-right: 10px;
        color: #4f46e5;
        text-decoration: none;
        font-size: 14px;
    }

    .footer {
        text-align: center;
        color: gray;
        margin-top: 40px;
        padding: 10px;
    }
</style>
</head>

<body>

<div class="container">

<header>
    <h1>Library Management System</h1>
    <nav>
        <button class="active">Dashboard</button>
        <button>Books</button>
        <button>Members</button>
        <button>Issue / Return</button>
    </nav>
</header>

<!-- Cards -->
<div class="cards">
    <div class="card">
        <div class="card-title">Books</div>
        <div class="card-number">12</div>
        <div>Total Titles</div>
    </div>

    <div class="card">
        <div class="card-title">Members</div>
        <div class="card-number">8</div>
        <div>Registered Members</div>
    </div>

    <div class="card">
        <div class="card-title">Issued</div>
        <div class="card-number">5</div>
        <div>Active Loans</div>
    </div>
</div>

<!-- Books Table -->
<div class="section-title">Books</div>
<table>
    <tr>
        <th>ID</th>
        <th>Title</th>
        <th>Author</th>
        <th>Copies</th>
        <th>Available</th>
        <th>Actions</th>
    </tr>

    <tr>
        <td>B_ABC1234</td>
        <td>Introduction to Algorithms</td>
        <td>Cormen</td>
        <td>3</td>
        <td>2</td>
        <td class="actions"><a href="#">Edit</a> <a href="#">Delete</a></td>
    </tr>

    <tr>
        <td>B_DEF5678</td>
        <td>Clean Code</td>
        <td>Robert C. Martin</td>
        <td>2</td>
        <td>1</td>
        <td class="actions"><a href="#">Edit</a> <a href="#">Delete</a></td>
    </tr>
</table>

<!-- Members Table -->
<div class="section-title">Members</div>
<table>
    <tr>
        <th>ID</th>
        <th>Name</th>
        <th>Email</th>
        <th>Phone</th>
        <th>Actions</th>
    </tr>

    <tr>
        <td>M_111AAAA</td>
        <td>Rajat Singh</td>
        <td>rajat@example.com</td>
        <td>9999999999</td>
        <td class="actions"><a href="#">Edit</a> <a href="#">Delete</a></td>
    </tr>

    <tr>
        <td>M_222BBBB</td>
        <td>Anita Sharma</td>
        <td>anita@example.com</td>
        <td>8888888888</td>
        <td class="actions"><a href="#">Edit</a> <a href="#">Delete</a></td>
    </tr>
</table>

<div class="footer">
    Made by <b>Rajat Singh</b> • Simple LMS • Static HTML & CSS
</div>

</div>
</body>
</html>
