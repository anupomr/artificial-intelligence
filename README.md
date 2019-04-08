﻿# artificial-intelligence implemented with Node.js and Express
 #First Page
<!DOCTYPE html>
<html>

<head>
  <title>
    <%= title %>
  </title>
  <!-- CSS section-->
  <link rel='stylesheet' href='bootstrap/dist/css/bootstrap.min.css' />
  <link rel="stylesheet" href="font-awesome/css/font-awesome.min.css">
  <link rel="stylesheet" href="public/Content/style.css">
</head>

<body>

  <header>
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
      <a class="navbar-brand" href="/"><img src="Assets/images/arlogo.png" height="40px"></a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">
          <% if(title=="Home"){%>
          <li class="nav-item active">
            <% } else {%>
          <li class="nav-item">
            <% } %>
            <a class="nav-link" href="/"><i class="fa fa-home"></i> Home <span class="sr-only">(current)</span></a>
          </li>
          <% if(title=="FeedBack"){%>
          <li class="nav-item active">
            <% } else {%>
          <li class="nav-item">
            <% } %>
            <a class="nav-link" href="/feedback"><i class="fa fa-comment"></i> Recognition</a>
          </li>
          <% if(title=="About"){%>
          <li class="nav-item active">
            <% } else {%>
          <li class="nav-item">
            <% } %>
            <a class="nav-link" href="/about"><i class="fa fa-info"></i> About</a>
          </li>
          <% if(title=="Logout"){%>
            <li class="nav-item active">
              <% } else {%>
            <li class="nav-item">
              <% } %>
              <a class="nav-link" href="/logout"> <i class="fa fa-lock"></i> Logout</a>
            </li>
        </ul>
        <form class="form-inline my-2 my-lg-0">
          <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
          <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
        </form>
      </div>
    </nav>

  </header>
  <main class="container">
    <!--Main Area-->
    <div class="jumbotron">
      <h1 class="display-4">Welcome to
        <%= title %>
      </h1>
      <p class="lead">This is a simple hero unit, a simple jumbotron-style component for calling extra attention to
        featured content or information.</p>

      <form action="/thanku" method="post">

        <fieldset class="style1" style="width: 497px">
          <legend>AI Info</legend>

          <table style="width: 103%">
            
            <tr>
              <td class="fieldLebel"> Sepal_length: </td>
              <td> <input type="number" step="any" size="30" name="sl"></td>
            </tr> 

            <tr>
              <td class="fieldLebel"> sepal_width: </td>
              <td> <input type="number" step="any" size="30" name="sw"></td>
            </tr> 
            <tr>
              <td class="fieldLebel"> petal_length: </td>
              <td> <input type="number" step="any" size="30" name="pl"></td>
            </tr> 
            <tr>
              <td class="fieldLebel"> petal_width: </td>
              <td> <input type="number" step="any" size="30" name="pw"></td>
            </tr> 

           

            <tr>
              <td></td>
              <td><input type="submit" class="btn btn-outline-success my-2 my-sm-0" value="Submit" name="Feedback"></td>
            </tr>
          </table>
        </fieldset>



      </form>

      <hr class="my-4">
      <p>This utility and content developed by Anupom Roy.</p>
      <a class="btn btn-primary btn-lg" href="https://www.linkedin.com/in/anupom-roy/" role="button">Learn more</a>
    </div>

  </main>


  <!-- JavaScript section-->
  <script src="jquery/dist/jquery.min.js"></script>
  <script src="bootstrap/dist/js/bootstrap.min.js"></script>
  <script src="Scripts/app.js"></script>
</body>

</html>


#Second Page
<!DOCTYPE html>
<html>

<head>
  <title>
    <%= title %>
  </title>
  <!-- CSS section-->
  <link rel='stylesheet' href='bootstrap/dist/css/bootstrap.min.css' />
  <link rel="stylesheet" href="font-awesome/css/font-awesome.min.css">
  <link rel="stylesheet" href="../public/Content/style.css">
</head>
  <body>
      <header>
          <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
            <a class="navbar-brand" href="/"><img src="Assets/images/arlogo.png" height="40px"></a>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent"
              aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
              <span class="navbar-toggler-icon"></span>
            </button>
      
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
              <ul class="navbar-nav mr-auto">
                <% if(title=="Home"){%>
                <li class="nav-item active">
                  <% } else {%>
                <li class="nav-item">
                  <% } %>
                  <a class="nav-link" href="/"><i class="fa fa-home"></i> Home <span class="sr-only">(current)</span></a>
                </li>
                <% if(title=="FeedBack"){%>
                <li class="nav-item active">
                  <% } else {%>
                <li class="nav-item">
                  <% } %>
                  <a class="nav-link" href="/feedback"><i class="fa fa-comment"></i> Recognition</a>
                </li>
                <% if(title=="About"){%>
                <li class="nav-item active">
                  <% } else {%>
                <li class="nav-item">
                  <% } %>
                  <a class="nav-link" href="/about"><i class="fa fa-info"></i> About</a>
                </li>
                <% if(title=="Logout"){%>
                  <li class="nav-item active">
                    <% } else {%>
                  <li class="nav-item">
                    <% } %>
                    <a class="nav-link" href="/logout"> <i class="fa fa-lock"></i> Logout</a>
                  </li>
              </ul>
              <form class="form-inline my-2 my-lg-0">
                <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
                <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
              </form>
            </div>
          </nav>
      
        </header>

        <main class="container">
            <!--Main Area-->
            <div class="jumbotron">
              <h1 class="display-4"> <%= title %>      </h1>
              <p class="lead">This is a simple  <%= title %> unit, a simple jumbotron-style component for calling extra attention to
                featured.</p>         
              
                <p>possibility of setosa is :<%= setosa %></p>
                <p>possibility of virginica is :<%= virginica %></p>
                <p>possibility of versicolor is :<%= versicolor %></p>
              <hr class="my-4">
              <p>This utility and content developed by Anupom Roy.</p>
              <a class="btn btn-primary btn-lg" href="https://www.linkedin.com/in/anupom-roy/" role="button">Learn more</a>
            </div>  
          </main>
    
    <!-- JavaScript section-->
  <script src="jquery/dist/jquery.min.js"></script>
  <script src="bootstrap/dist/js/bootstrap.min.js"></script>
  <script src="Scripts/app.js"></script>
  </body>
</html>
