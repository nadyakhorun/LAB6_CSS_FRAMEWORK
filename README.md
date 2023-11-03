# LAB6_CSS_FRAMEWORK

Nama          : Nadya Khairunnisa

NIM           : 312210133

Kelas         : TI.22.A.1

# Instruksi Praktikum

1. Persiapkan text editor misalnya VSCode.
   
2. Buat folder baru dengan nama lab6_css_framework
   
3. Buat file baru dokumen html
   
4. Buat struktur dasar dari dokumen HTML.
   
5. Buatlah layout web sederhana menggunakan css frameword (Twitter Bootsrtap).
    
6. Lakukan validasi dokumen html dengan mengakses http://validator.w3.org

# Langkah-Langkah

1. Pertama kita buat file dengan nama file jQueryEffects_Sliding.html

2. Selanjutnya kita masukan codingan seperti berikut.

        <!DOCTYPE html>
        <html>
        <head>
            <script src="http://ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js">
            </script>
            <script>
            $(document).ready(function(){
                $("#flip").click(function(){
                    $("#panel").slideToggle("slow");
                });
            });
            </script>
        
            <style type="text/css">
            #panel, #flip {
                padding:5px;
                text-align:center;
                background-color: #e5eecc;
                border:solid 1px #c3c3c3;
            }
            #panel {
                padding:50px;
                display:none;
            }
            </style>
        </head>
        <body>
            <div id="flip">Click to slide the panel down or up</div>
            <div id="panel">Hello World!</div>
        </body>
        </html>

![hasil web 0](https://github.com/nadyakhorun/LAB6_CSS_FRAMEWORK/assets/115801823/409de5fd-81ce-4202-b475-39ebe60d8629)

3. Kemudian kita lakukan run pada browser untuk melihat hasil dari codingan tersebut seperti berikut.

![hasil web 1](https://github.com/nadyakhorun/LAB6_CSS_FRAMEWORK/assets/115801823/7253bd00-87e2-406a-b01e-391f69668d16)

![hasil web 2](https://github.com/nadyakhorun/LAB6_CSS_FRAMEWORK/assets/115801823/36c2484d-0251-48c5-9ee7-af5713deb371)

4. Selanjutnya kita membuat file baru lagi dengan nama file jQueryEffects_Animation.html

5. Kemudian kita masukan codingan seperti berikut.

          <!DOCTYPE html>
          <html>
          <head>
              <script src="http://ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js">
              </script>
              <script>
              $(document).ready(function(){
                  $("button").click(function(){
                      var div=$("div");
                      div.animate({height:'300px',opacity:'0,4'},"slow");
                      div.animate({width:'300px',opacity:'0,8'},"slow");
                      div.animate({height:'100px',opacity:'0,4'},"slow");
                      div.animate({width:'100px',opacity:'0,8'},"slow");
                  });
              });
              </script>
              </head>
              
              <body>
                  <button>Start Animation</button>
                  <div style="background:#98bf21;height:100px;width:100px;position:absolute;">
                  </div>
              </body>
              </html>
   
![hasil web 3](https://github.com/nadyakhorun/LAB6_CSS_FRAMEWORK/assets/115801823/07b2697c-c84c-45f3-be8b-0e50707efcad)

6. Selanjutnya kita lakukan run kembali untuk melihat hasilnya seperti berikut.

![hasil web 4](https://github.com/nadyakhorun/LAB6_CSS_FRAMEWORK/assets/115801823/0e0f31eb-ae97-4748-a1b7-7892ec740de5)

![hasil web 5](https://github.com/nadyakhorun/LAB6_CSS_FRAMEWORK/assets/115801823/6082cb1f-82eb-487c-8a95-ff239f9490f7)

7. Kemudian kita buat file baru lagi dengan nama file jQueryUIDraggable.html

8. Selanjutnya kita masukan codingan seperti berikut

              <html lang="en">
              <head>
                  <script src="http://code.jquery.com/jquery-1.9.1.js"></script>
                  <script src="http://code.jquery.com/ui/1.10.3/jquery-ui.js"></script>
                  <style>
                  #draggable {
                      width: 125px;
                      height: 125px;
                      background-color: #FFF;
                      text-align: center;
                      padding: 1px 5px;
                      border: 1px solid #AAA;
                      margin: auto;
                      float: left;
                  }
                  #containment-wrapper {
                      width: 95%;
                      height: 200px;
                      border: 1px solid #4E4E4E;
                      padding: 10px;
                  }
                  </style>
                  <script>
                  $(function (){
                      $("#draggable").draggable({
                          containment: "#containment-wrapper",scroll:false
                      })
                  })
                  </script>
              </head>
              <body>
                  <div id="containment-wrapper">
                      <div id="draggable">
                          <p>I'm contained within the box</p>
                      </div>
                  </div>
              </body>
              </html>

![hasil web 6 1](https://github.com/nadyakhorun/LAB6_CSS_FRAMEWORK/assets/115801823/a6b559bf-1b81-464b-b366-34eabc823f5a)

![hasil web 6](https://github.com/nadyakhorun/LAB6_CSS_FRAMEWORK/assets/115801823/1f518f91-2be1-41a1-8ea0-2f51771adcbb)

9. Kemudian kita lakukan run pada browser untuk melihat hasilnya seperti berikut

![hasil web 7](https://github.com/nadyakhorun/LAB6_CSS_FRAMEWORK/assets/115801823/c35e2fff-240e-4a49-8318-62d8493ba295)

# TWITTER BOOTSTRAP

Disini kita akan membuat layout sederhana dengan menggunakan css frameword(Twitter Bootstrap).

1. Kita akan membuat file nya terlebih dahulu dengan nama Twitter_Bootstrap

2. Kemudian kita masukan codingannya seperti berikut.

            <!doctype html>
            <html lang="en">
                <head>
                    <!--Required Meta Tags-->
                    <meta charset="utf-8">
                    <meta name="viewport" content="width=device-width, initial-scale=1">
                    
                    <!--Bootstrap CSS-->
                    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">
                    <title>Layout Sederhana</title>
                </head>
                <body>
                    <!--Container Start-->
                    <div class="container shadow-lg">
                        <!--Heading Start-->
                        <div class="card-body bg-light p-3">
                            <h1 class="text-secondary py-3 text-opacity-50 fw-bold">Layout Sederhana</h1>
                        </div>
                        <!--Heading End-->
            
                        <!--Navbar Start-->
                        <nav class="navbar navbar-expand-lg navbar-dark" style="background-color: #1f5faa;">
                            <div class="container-fluid">
                            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                                <span class="navbar-toggler-icon"></span>
                            </button>
                            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                                <ul class="navbar-nav">
                                <li class="nav-item active ms-4">
                                    <a class="nav-link text-light fs-5 fw-semibold" aria-current="page" href="index.html" >Home</a>
                                </li>
                                <li class="nav-item ms-4">
                                    <a class="nav-link fs-5 fw-semibold" href="#">Article</a>
                                </li>
                                <li class="nav-item ms-4">
                                    <a class="nav-link fs-5 fw-semibold" href="#">About</a>
                                </li>
                                <li class="nav-item ms-4">
                                    <a class="nav-link fs-5 fw-semibold" href="#">Contact</a>
                                </li>
                                </ul>
                            </div>
                            </div>
                        </nav>
                        <!--Navbar End-->
            
                        <!--Jumbotron Start-->
                        <div class="jumbotron p-2 text-secondary bg-opacity-25" style="background-color:#e4e4e5;">
                            <h1 class="p-3 text-secondary fw-bold">Hello World!</h1>
                            <p class="lead p-3 text-secondary">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p>
                            <a href="#" class="btn btn-primary mb-3 fw-semibold mx-3">Learn more &raquo;</a></p>
                        </div>
                        <!--Jumbotron End-->
            
                         <!--Row Start-->
                         <div class="row">
                            <!--Box Start-->
                            <div class="col-md-9">
                                <div class="row">
                                    <div class="col-3 mx-4">
                                        <div class="col mt-4">
                                            <div class="card pt-3" style="border: 0;">
                                                <img src="https://dummyimage.com/120/db7d25/fff.png" class="card-img-top rounded-circle" alt="...">
                                                <div class="card-body">
                                                    <h5 class="card-title text-center">Heading</h5>
                                                    <p class="card-text text-center">Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
                                                    <p class="card-text text-center"><a href="#" class="btn btn-secondary mt-2">View Detail</a></p>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="col-3 mx-4">
                                        <div class="col mt-4">
                                            <div class="card pt-3" style="border: 0;">
                                                <img src="https://dummyimage.com/120/3e73e6/fff.png" class="card-img-top rounded-circle" alt="...">
                                                <div class="card-body">
                                                    <h5 class="card-title text-center">Heading</h5>
                                                    <p class="card-text text-center">Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
                                                    <p class="card-text text-center"><a href="#" class="btn btn-secondary mt-2">View Detail</a></p>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="col-3 mx-4">
                                        <div class="col mt-4">
                                            <div class="card pt-3" style="border: 0;">
                                                <img src="https://dummyimage.com/120/71e6d4/fff.png" class="card-img-top rounded-circle" alt="...">
                                                <div class="card-body">
                                                    <h5 class="card-title text-center">Heading</h5>
                                                    <p class="card-text text-center">Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
                                                    <p class="card-text text-center"><a href="#" class="btn btn-secondary mt-2">View Detail</a></p>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <!--Box End-->
            
                            <!--Widget Start-->
                            <div class="col-md-3">
                                <div class="my-3 mt-5">
                                    <div class="list-group" style="border-radius: 0;">
                                        <a href="#" class="list-group-item list-group-item-action active" aria-current="true" style="font-weight: bold;">Widget Header</a>
                                        <a href="#" class="list-group-item list-group-item-action">Widget Link</a>
                                        <a href="#" class="list-group-item list-group-item-action">Widget Link</a>
                                        <a href="#" class="list-group-item list-group-item-action">Widget Link</a>
                                        <a href="#" class="list-group-item list-group-item-action">Widget Link</a>
                                        <a href="#" class="list-group-item list-group-item-action">Widget Link</a>
                                    </div>
                                    <div class="list-group my-4" style="border-radius: 0; border: 1px">
                                        <a href="#" class="list-group-item list-group-item-action active " aria-current="true" style="font-weight: bold;">Widget Text</a>
                                        <a href="#" class="list-group-item list-group-item-action">
                                            <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p>
                                        </a>
                                    </div>
                                </div>
                            </div>
                            <!--Widget End-->
            
                            <!--Divider Start-->
                            <div>
                                <!--Section 1-->
                                <div class="mb-5" style="width: 900px; border: 0;">
                                    <h2>First featurette heading.</h2>
                                    <div class="row no-gutters">
                                        <div class="col-md-3">
                                            <img src="https://dummyimage.com/150/7b8a70/fff.png" class="card-img-top rounded-square" style="width: 200px;" alt="...">
                                        </div>
                                        <div class="col-md-8">
                                            <div class="card-body">
                                                <p class="card-text lead p-3 fs-5">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <!--Section 2-->
                                <div class="mt-5 mb-5" style="width: 900px; border: 0;">
                                    <h2>First featurette heading.</h2>
                                    <div class="row">
                                        <div class="col-md-8">
                                            <div class="card-body">
                                                <p class="lead p-3 fs-5">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p>
                                            </div>
                                        </div>
                                        <div class="col-md-3">
                                            <img src="https://dummyimage.com/150/7b8a70/fff.png" class="card-img-top rounded-square" style="width: 200px;" alt="...">
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <!--Divider End-->
            
                            <!--Footer Start-->
                            <div class="card-footer text-start bg-dark text-light p-2">
                                <p>&copy; 2021 - Universitas Pelita Bangsa</p>
                            </div>
                            <!--Footer End-->
            
                        </div>
                        <!--Row End-->
            
                    </div>
                    <!--Container End-->
            
                    <!--Bootstrap Bundle with Popper-->
                    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL" crossorigin="anonymous"></script>
                </body>
            </html>

3. Kemudian kita lakukan run ke browser untuk melihat hasil layout sederhana seperti berikut

![hasil akhir banget](https://github.com/nadyakhorun/LAB6_CSS_FRAMEWORK/assets/115801823/6d608e2a-fa1f-490d-9a20-ba713870abcd)

# Sekian, Terima Kasih
