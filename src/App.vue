<template>
  <div id="app">
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <a class="navbar-brand" href="#">Student Portal</a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">
          <li class="nav-item active">
            <a class="nav-link" href="/">Home <span class="sr-only">(current)</span></a>
          </li>
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
              Dropdown
            </a>
            <div class="dropdown-menu" aria-labelledby="navbarDropdown">
              <router-link class="dropdown-item" to="/update">Update Resume</router-link>
              <div class="dropdown-divider"></div>
              <router-link class="dropdown-item" to="/signup">Sign up</router-link>
              <router-link class="dropdown-item" to="/signin">Sign In</router-link>
              <router-link class="dropdown-item" to="/logout">Log out</router-link>

 
            </div>
          </li>
        </ul>
        <form class="form-inline my-2 my-lg-0">
          <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
          <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
        </form>
      </div>
    </nav>
    <div class="container">
         <router-view/>

</div>


    <footer class="bg-gray-dark">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col text-center">
                    <ul class="m-0 p-0">
                        <li class="list-inline-item">
                            <a href="#" target="_blank" class="bg-gray-2 box-shadow-wide rounded text-white text-extra-large">
                                <i class="fa fa-facebook ease"></i>
                            </a>
                        </li>
                        <li class="list-inline-item">
                            <a href="#" target="_blank" class="bg-gray-2 box-shadow-wide rounded text-white text-extra-large">
                                <i class="fa fa-twitter ease"></i>
                            </a>
                        </li>
                        <li class="list-inline-item">
                            <a href="#" target="_blank" class="bg-gray-2 box-shadow-wide rounded text-white text-extra-large">
                                <i class="fa fa-linkedin ease"></i>
                            </a>
                        </li>
                    </ul>
                    
                    <p class="m-0 mt-4 text-gray text-medium">&copy; 2017 Nick Berg. All rights reserved.</p>
                </div>
                <!-- //.col -->
            </div>
            <!-- //.row -->
        </div>
        <!-- //.container -->
    </footer>
  </div>
</template>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  /*text-align: center;*/
  color: #2c3e50;
}
</style>
