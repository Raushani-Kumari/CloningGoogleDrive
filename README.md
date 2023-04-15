# CloningGoogleDrive
#I am pleased to share that I have successfully cloned Google Drive using HTML and CSS.

#html code

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <!-- Compiled and minified CSS -->
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/materialize/1.0.0/css/materialize.min.css"
    />

    <link
      href="https://fonts.googleapis.com/icon?family=Material+Icons"
      rel="stylesheet"
    />

    <link rel="stylesheet" href="style.css" />
    <title>Google Drive</title>
  </head>
  <body>
    <div class="navbar-fixed">
      <nav class="nav-extended white">
        <div class="nav-wrapper white">
          <ul>
            <li>
              <a href="#!" class="title grey-text text-darken-1"
                >Google Drive
              </a>
            </li>
          </ul>
          <div class="search-wrapper">
            <i class="material-icons">search</i>
            <input type="search" name="Search" placeholder="Search Drive" />
          </div>
          <ul class="right">
            <li>
              <a href="#!">
                <i class="material-icons grey-text text-darken-1">apps</i>
              </a>
            </li>
            <li>
              <a href="#!">
                <i class="material-icons grey-text text-darken-1"
                  >notifications</i
                >
              </a>
            </li>
            <li>
              <a href="#!">
                <img
                  src="google_drive_logo.png"
                  alt="profile pic"
                  class="circle"
                />
              </a>
            </li>
          </ul>
        </div>
        <div class="nav-wrapper nav-2">
          <ul>
            <li>
              <a
                href="#!"
                class="waves-effect waves-light btn btn-flat white-text"
                >New</a
              >
            </li>
          </ul>
          <ul class="right">
            <li>
              <a href="#!">
                <i class="material-icons grey-text text-darken-1"> view_list</i>
              </a>
            </li>
            <li>
              <a href="#!">
                <i class="material-icons grey-text text-darken-1">info</i>
              </a>
            </li>
            <li>
              <a href="#!">
                <i class="material-icons grey-text text-darken-1">settings</i>
              </a>
            </li>
          </ul>
        </div>
      </nav>
    </div>
    <ul class="side-nav fixed floating transparent z-depth-0">
      <li class="active">
        <a href="#">
          <i class="material-icons blue-text text-darken-1">dashboard</i>My
          Drive
        </a>
      </li>
      <li>
        <a href="#"><i class="material-icons">devices</i>Computers</a>
      </li>
      <li>
        <a href="#"><i class="material-icons">people</i>Shared with me</a>
      </li>
      <li>
        <a href="#"><i class="material-icons">access_time</i>Recent</a>
      </li>
      <li>
        <a href="#"><i class="material-icons">camera</i>Google Photos</a>
      </li>
      <li>
        <a href="#"><i class="material-icons">star</i>Starred</a>
      </li>
      <li>
        <a href="#"><i class="material-icons">delete</i>Trash</a>
      </li>
      <li><div class="divider"></div></li>
      <li>
        <a href="#"><i class="material-icons">storage</i>Upgrade storage</a>
      </li>
    </ul>
    <div class="main">
      <div class="container-fluid">
        <p class="subheader">Folders</p>
        <div class="card-panel folder">
          <i class="material-icons left">folder</i>Folder
        </div>
        <div class="card-panel folder">
          <i class="material-icons left">folder</i>Folder
        </div>
        <div class="card-panel folder">
          <i class="material-icons left">folder</i>Folder
        </div>
      </div>
    </div>
  </body>
  <!-- Compiled and minified JavaScript -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/materialize/1.0.0/js/materialize.min.js"></script>
</html>



#css code
body {
  background-color: #f0f0f0;
  font-size: 13px;
}
.card,
.card-panel {
  padding: 15px, 20px;
  box-shadow: 0 1px 4px 0 rgba(0, 0, 0, 0.14);
}
.container-fluid {
  padding: 1rem 2.5rem;
  margin: auto;
}
.row {
  margin: 0, -0.75rem;
}
.main {
  position: absolute;
  width: calc(100%-250px);
  top: 125px;
  margin-left: 250px;
}
.subheader {
  color: rgba(0, 0, 0, 0.54);
  font-weight: 500;
}
/* nav */
nav {
  box-shadow: 0 1px 8px rgba(0, 0, 0, 0.3);
}
nav ul li {
  text-align: center;
}
nav ul.right {
  padding: 12px;
}
nav ul.right li {
  max-width: 48px;
}
nav ul a {
  padding-right: 0 12px;
}
nav ul a img {
  height: 32px;
  width: 32px;
  vertical-align: middle;
  margin-left: -5px;
}
.nav-wrapper {
  padding-left: 12px;
}
.nav-wrapper ul a:hover {
  background-color: transparent;
}
.nav-wrapper .title {
  font-size: 1.4rem;
}
.nav-wrapper .btn-flat {
  background-color: #4285f4 !important;
  font-size: 13px;
  font-weight: 500;
  height: 30px;
  line-height: 30px;
  width: 94px;
}
.nav-2,
.nav-2 i {
  height: 56px !important;
  line-height: 56px !important;
  min-height: 56px !important;
}
.search-wrapper {
  margin: 10px auto 0 170px;
  width: calc(100%- 450px);
  max-width: 650px;
  height: 46px;
  position: fixed;
}
.search-wrapper i {
  color: #757575;
  position: absolute;
  font-size: 24px;
  top: 5px;
  left: 24px;
  line-height: 36px !important;
}
input[type="search"]:not(.browser-default) {
  display: block;
  padding: 11px 8px 11px 72px;
  width: 100%;
  background: #f5f5f5;
  height: 24px;
  border: none;
  font-size: 16px;
  outline: none;
  border-radius: 2px;
  color: #757575;
}
input[type="search"]:focus {
  border-bottom: none !important;
  box-shadow: none !important;
}
input[type="search"]::placeholder {
  color: #757575;
}
/* sidenav */
.side-nav.floating {
  width: 250px;
  padding: 85px 8px 0 !important;
  height: calc(100%-130px);
  left: initial;
  right: initial;
  top: 125px;
  transform: initial;
  z-index: auto;
  margin: 0.5rem 0 1rem 0;
  border-radius: 2px;
  background: transparent;
  box-shadow: none;
}
.side-nav .divider {
  margin: 8px 0;
}
.side-nav .active {
  background-color: rgba(0, 0, 0, 0.05);
}
.side-nav .active a {
  color: #212121;
  font-weight: 500;
}
.side-nav .subheader {
  line-height: 24px;
  height: 32px;
  margin: 0;
  padding: 4px 16px;
  color: #616161;
  font-weight: normal;
  font-size: 13px;
}
.side-nav li a,
.side-nav li a i.material-icons {
  height: 40px;
  line-height: 40px;
}
.side-nav li a i.material-icons {
  margin-right: 24px;
}
.side-nav li a {
  padding: 0 16px;
  font-weight: normal;
  font-size: 13px;
  color: #616161;
}
side-nav li a:hover {
  border-radius: 2px;
}
/* folders */
.folder {
  width: 185px;
  display: inline-block;
  margin: 15px 20px 15px 0;
  font-weight: 500;
}
.folder i {
  color: rgba(0, 0, 0, 0.54);
  margin-top: -3px;
}


