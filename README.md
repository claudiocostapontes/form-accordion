<!DOCTYPE html>
<html lang="pt-br">

<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Formulário Accordion</title>

  <!-- CSS Bootstrap -->

  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet"
    integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">

  <!-- CSS Externo -->
  <link href="css/estilo.css" rel="stylesheet" type="text/css" media="all" />


</head>

<body>

  <!-- Navbar -->

  <header>
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
      <div class="container-fluid">
        <a class="navbar-brand" href="#">Navbar</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#">Home</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Link</a>
            </li>
            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-bs-toggle="dropdown"
                aria-expanded="false">
                Dropdown
              </a>
              <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
                <li><a class="dropdown-item" href="#">Action</a></li>
                <li><a class="dropdown-item" href="#">Another action</a></li>
                <li>
                  <hr class="dropdown-divider">
                </li>
                <li><a class="dropdown-item" href="#">Something else here</a></li>
              </ul>
            </li>
            <li class="nav-item">
              <a class="nav-link disabled">Disabled</a>
            </li>
          </ul>
          <!-- Início do Modal -->
          <!-- Button trigger modal -->
          <button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal">
            Login
          </button>

          <!-- Modal -->

          <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel"
            aria-hidden="true">
            <div class="modal-dialog">
              <div class="modal-content">
                <div class="modal-header">
                  <h5 class="modal-title" id="exampleModalLabel">Fazer Login</h5>
                  <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                  <form action="" method="">
                    <div class="input-group mb-3">
                      <span class="input-group-text" id="inputGroup-sizing-default">Usuário</span>
                      <input type="text" class="form-control" aria-label="Sizing example input"
                        aria-describedby="inputGroup-sizing-default">
                    </div>
                  </form>
                </div>
                <div class="modal-body">
                  <form action="" method="">
                    <div class="input-group mb-3">
                      <span class="input-group-text" id="inputGroup-sizing-default">Senha</span>
                      <input type="password" class="form-control" aria-label="Sizing example input"
                        aria-describedby="inputGroup-sizing-default">
                    </div>
                </div>
                <div class="modal-footer">
                  <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Fechar</button>
                  <button type="button" class="btn btn-primary">Entrar</button>
                  </form>
                </div>
              </div>
            </div>
          </div>
          <!-- Fim do Modal -->
        </div>
      </div>
    </nav>
  </header>

  <!-- Conteúdo -->

  <main>
    <hr />
    <div class="container">
      <h1>Formulário Accordion</h1>
      <hr />
      <hr />
      <form action="" method="">
        <div class="accordion" id="accordionExample">
          <div class="accordion-item">
            <h2 class="accordion-header" id="headingOne">
              <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne"
                aria-expanded="true" aria-controls="collapseOne">
                <strong>Dados Pessoais</strong>
              </button>
            </h2>
            <div id="collapseOne" class="accordion-collapse collapse show" aria-labelledby="headingOne"
              data-bs-parent="#accordionExample">
              <div class="accordion-body">
                <div class="input-group mb-3">
                  <span class="input-group-text">Nome</span>
                  <input type="text" aria-label="First name" class="form-control">
                  <span class="input-group-text">Sobrenome</span>
                  <input type="text" aria-label="Last name" class="form-control">
                </div>
                <div class="input-group mb-3">
                  <span class="input-group-text">RG</span>
                  <input type="text" aria-label="First name" class="form-control">
                  <span class="input-group-text">CPF</span>
                  <input type="text" aria-label="Last name" class="form-control">
                </div>
                <div class="input-group mb-3">
                  <span class="input-group-text">Data de Nascimento</span>
                  <input type="date" aria-label="Data de Nascimento" class="form-control">
                  <label class="input-group-text" for="inputGroupSelect01">Gênero</label>
                  <select class="form-select" id="inputGroupSelect01">
                    <option selected>Escolha uma Opção</option>
                    <option value="1">Masculino</option>
                    <option value="2">Feminino</option>
                    <option value="3">Outro</option>
                  </select>
                </div>
              </div>
            </div>
          </div>
          <div class="accordion-item">
            <h2 class="accordion-header" id="headingTwo">
              <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
                data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
                <strong>Endereço</strong>
              </button>
            </h2>
            <div id="collapseTwo" class="accordion-collapse collapse" aria-labelledby="headingTwo"
              data-bs-parent="#accordionExample">
              <div class="accordion-body">
                <div class="input-group mb-3">
                  <label class="input-group-text" for="inputGroupSelect01">Bairro</label>
                  <select class="form-select" id="inputGroupSelect01">
                    <option selected>Escolha um Bairro</option>
                    <option value="1">Taguatinga</option>
                    <option value="2">Ceilância</option>
                    <option value="3">Gama</option>
                    <option value="4">Asa Sul</option>
                    <option value="5">Asa Norte</option>
                    <option value="6">Cruzeiro</option>
                    <option value="7">Guará</option>
                    <option value="8">Águas Claras</option>
                    <option value="9">Vicente Pires</option>
                  </select>
                  <span class="input-group-text" id="inputGroup-sizing-default">CEP</span>
                  <input type="text" class="form-control" aria-label="Sizing example input"
                    aria-describedby="inputGroup-sizing-default">
                </div>
                <div class="input-group mb-3">
                  <span class="input-group-text" id="inputGroup-sizing-default">Município</span>
                  <input type="text" class="form-control" aria-label="Sizing example input"
                    aria-describedby="inputGroup-sizing-default"> <label class="input-group-text"
                    for="inputGroupSelect01">UF</label>
                  <select class="form-select" id="inputGroupSelect01">
                    <option selected>Escolha uma Opção</option>
                    <option value="1">DF</option>
                    <option value="2">GO</option>
                    <option value="3">MT</option>
                    <option value="3">MS</option>
                  </select>
                </div>
              </div>
            </div>
          </div>
          <div class="accordion-item">
            <h2 class="accordion-header" id="headingThree">
              <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
                data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
                Accordion Item #3
              </button>
            </h2>
            <div id="collapseThree" class="accordion-collapse collapse" aria-labelledby="headingThree"
              data-bs-parent="#accordionExample">
              <div class="accordion-body">
                <strong>This is the third item's accordion body.</strong> It is hidden by default, until the collapse
                plugin adds the appropriate classes that we use to style each element. These classes control the overall
                appearance, as well as the showing and hiding via CSS transitions. You can modify any of this with
                custom CSS or overriding our default variables. It's also worth noting that just about any HTML can go
                within the <code>.accordion-body</code>, though the transition does limit overflow.
              </div>
            </div>
          </div>
        </div>
      </form>
    </div>
  </main>

  <!-- JS Bootstrap -->

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"
    integrity="sha384-ka7Sk0Gln4gmtz2MlQnikT1wXgYsOg+OMhuP+IlRH9sENBO0LRn5q+8nbTov4+1p"
    crossorigin="anonymous"></script>

</body>

</html>
