
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Lebenslauf</title>
    <link href="../Stylesheet.css" rel="stylesheet" />
    <script src="Jquery.js"></script>
  </head>
  <body>
    <div id="UP_Btn"></div>
    <div class="body">
      <div id="Header">
        <img src="Image/Al.jpg" id="p_pic" />
        <h1>Alihossain Ahmadi</h1>
        <h2>alihossain.ahmadi@hotmail.com</h2>
        <h2>(+49) 01623 452 463</h2>
        <h2>Elfenhang 13 , 42329 Wuppertal</h2>
      </div>
      <div class="Menu">
        <h3 class="Menu_Tp" id="Home">Home</h3>
        <h3 class="Menu_Tp" id="Carrier">Fähigkeiten</h3>
        <h3 class="Menu_Tp" id="project">Project</h3>
        <h3 class="Menu_Tp" id="About">Über mich</h3>
        <input type="search" id="Searchbox" placeholder="Search ..." />
      </div>
      <div id="Content">
        <div class="cont_all" id="Home1" style="display: none"></div>
        <div class="cont_all" id="Carrier1" style="display: inline">
          <h4>
            <li>Html 5</li>
            <li>Css</li>
            <li>JQuery.js</li>
            <li>React.js</li>
            <li>Node.js</li>
            <li>Bootstrap</li>
            <li>TailwindCss</li>
            <li>Asp.net MVC</li>
            <li>PHP</li>
            <li>MS Sql</li>
            <li>My Sql</li>
            <li>Und erste Erfahrung mit</li>
            <li>C++</li>
            <li>C#</li>
            <li>JavaScript</li>
          </h4>
        </div>
        <div class="cont_all" id="project1" style="display: none">
          <div class="project">
            <div class="sing_proj">
              <a href="https://www.haerigroup.com//" target="_blank">
                <img src="Image/8p.jpg" alt="mashhaddpu" class="pic_proj" />
              </a>
            </div>
            <div class="sing_proj">
              <a href="http://www.jpgc.ir/" target="_blank">
                <img src="Image/9p.jpg" alt="mashhaddpu" class="pic_proj" />
              </a>
            </div>
            <div class="sing_proj">
              <a href="http://mashhaddpu.com/default.aspx" target="_blank">
                <img src="Image/1p.jpg" alt="mashhaddpu" class="pic_proj" />
              </a>
            </div>
            <div class="sing_proj">
              <a href="https://mahampg.ir/" target="_blank">
                <img src="Image/7p.jpg" alt="mashhaddpu" class="pic_proj" />
              </a>
            </div>
            <div class="sing_proj">
              <a href="http://www.fhp.co.ir/" target="_blank">
                <img src="Image/6p.jpg" alt="mashhaddpu" class="pic_proj" />
              </a>
            </div>
            <div class="sing_proj">
              <a href="https://www.armanrazavi-ihe.ac.ir//" target="_blank">
                <img src="Image/3p.jpg" alt="mashhaddpu" class="pic_proj" />
              </a>
            </div>
            <div class="sing_proj">
              <a href="https://seebarghotel.com/" target="_blank">
                <img src="Image/4p.jpg" alt="mashhaddpu" class="pic_proj" />
              </a>
            </div>
            <div class="sing_proj">
              <a href="http://faragaman.shop/" target="_blank">
                <img src="Image/5p.jpg" alt="mashhaddpu" class="pic_proj" />
              </a>
            </div>
            <div class="sing_proj">
              <a href="http://www.mashhad-cinema.ir/" target="_blank">
                <img src="Image/2p.jpg" alt="mashhaddpu" class="pic_proj" />
              </a>
            </div>
          </div>
        </div>
        <div class="cont_all" id="About1" style="display: none">
          <h4>
            Hi ,<br />
            Ich bin Alihossain ,geboren am 28. Mai 1994 in Maschad Iran . Ich
            habe im Jahr 2012 meine Abitur gemacht und ein Jahr später konnte
            ich die Universitätsprüfung als Software-Enginuer ablegen . <br />
            während meinen Studien habe ich an einem CIW-Kurs teilgenommen, um
            meine Programmierkenntnisse zu erweitern <br />
            Nach dem dritten Semester habe ich meine Studium abgebrochen und bin
            nach Deutschland gekommen <br /><br />
            Meine Muttersprache ist Persisch und ich kann Deutsch und Englisch
            als Fremdsprachen sprechen <br /><br />Meine Hobbys sind Bücher
            lesen und fahrradfahren , damit ich mich besser konzentrieren kann .
          </h4>
        </div>
      </div>
      <div id="Footer">
        <h6>Powered by Ahmadi</h6>
      </div>
      <div style="position: relative; background-color: aquamarine"></div>
    </div>
  </body>
</html>
<script>
  $(window).scroll(function () {
    var height = $(window).scrollTop();
    if (height >= 260) {
      $("#UP_Btn").fadeIn();
    } else {
      $("#UP_Btn").fadeOut();
    }
  });

  $(".Menu_Tp").click(function () {
    var IDd = $(this).attr("id");
    $("html, body").animate({ scrollTop: 260 }, "slow");
    $(".cont_all").css("display", "none");
    $("#" + IDd + "1").css("display", "inline");
  });

  $("#UP_Btn").click(function () {
    $("html, body").animate({ scrollTop: 0 }, "slow");
  });
</script>
