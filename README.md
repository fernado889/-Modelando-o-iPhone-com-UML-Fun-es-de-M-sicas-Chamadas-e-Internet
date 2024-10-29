# -Modelando-o-iPhone-com-UML-Fun-es-de-M-sicas-Chamadas-e-Internet
classDiagram

  class iPhone {

    - musicaAtual: String

    - numeroTelefone: String

    - urlAtual: String

    + tocar()

    + pausar()

    + selecionarMusica(String musica)

    + ligar(String numero)

    + atender()

    + iniciarCorreioVoz()

    + exibirPagina(String url)

    + adicionarNovaAba()

    + atualizarPagina()

  }



  interface ReprodutorMusical {

    + tocar()

    + pausar()

    + selecionarMusica(String musica)

  }



  interface AparelhoTelefonico {

    + ligar(String numero)

    + atender()

    + iniciarCorreioVoz()

  }



  interface NavegadorInternet {

    + exibirPagina(String url)

    + adicionarNovaAba()

    + atualizarPagina()

  }



  iPhone ..> ReprodutorMusical

  iPhone ..> AparelhoTelefonico

  iPhone ..> NavegadorInternet
