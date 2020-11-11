# BaseScreen usando BottomNavigationBar para navegação entre telas.


BottomNavigationBar usando a biblioteca https://pub.dev/packages/bottom_navy_bar, com animação nativa: curve: Curves.elasticOut, animationDuration: Duration(milliseconds: 1100).
Usando navegação com PageView: physics: NeverScrollableScrollPhysics => Evitar a navegação arrastando a tela para os lados. 
Controlador para os BottomNavyBarItem e o PageView: PageController _pageController;
  int _page = 0; => Variavel para definir as paginas.
  @override
  void initState() {
    super.initState();
    _pageController = PageController();
  }

  @override
  void dispose() {
    _pageController.dispose();
    super.dispose();
  }


