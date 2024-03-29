# Materiais de aprendizado para estudar Qt
Este repositório contém materiais para estudar Qt em português e inglês.

## Índice

* Introdução
  * [O que é o Qt? Como posso usar o Qt?](#o-que-%C3%A9-o-qt-como-posso-usar-o-qt)
  * [Qual a diferença entre QtCore, QtWidgets, QtQuick e QML?](#qual-a-diferen%C3%A7a-entre-qtcore-qtwidgets-qtquick-e-qml)
  * [Que linguagens posso usar para desenvolver em Qt?](#que-linguagens-posso-usar-para-desenvolver-em-qt)
  * [Onde/como posso ler a documentação da API do Qt?](#ondecomo-posso-ler-a-documenta%C3%A7%C3%A3o-da-api-do-qt)

* Comece aqui
  * [Rota de aprendizado para iniciantes](#rota-de-aprendizado-para-iniciantes)

* Recursos
  * [Canais para seguir](#canais-para-seguir)
  * [Introduções ao Qt](#introdu%C3%A7%C3%B5es-ao-qt)
  * [Cursos completos de Qt](#cursos-completos-de-qt)
  * [Livros para aprender Qt](#livros-para-aprender-qt)
  * [Tutoriais de Qt oficiais da The Qt Company em Inglês](#tutoriais-de-qt-oficiais-da-the-qt-company-em-ingl%C3%AAs)
  * [Talks de Qt oficiais da The Qt Company em Inglês (material opcional)](#talks-de-qt-oficiais-da-the-qt-company-em-ingl%C3%AAs-material-opcional)

* Módulos
  * [QtCore](#qtcore-1)
  * [QtWidgets](#qtwidgets-1)
  * [QtQuick](#qtquick)
  * [PySide/PyQt](#pysidepyqt)

* Mais
  * [Outros links](#outros-links)
  * [Contribuindo](#contribuindo)

## O que é o Qt? Como posso usar o Qt?

<details>
  <summary>Clique aqui para ler</summary>
  
O [Qt](https://www.qt.io/) (pronunciado [/kjuːt/](https://upload.wikimedia.org/wikipedia/commons/7/73/En-us-cute.ogg), como a palavra cute do inglês) é um framework utilizado para criar aplicativos modernos para desktop, dispositivos móveis e embarcados. Ele é feito em C++ e permite escrever um mesmo código para múltiplas plataformas, como Linux, Windows, Mac e Android, dentre outros.

O Qt extende o C++ e torna ele mais agradável para criar suas aplicações gráficas, e fornece também uma linguagem própria declarativa altamente produtiva, o QML. Ele inclui vários módulos, dentre eles o QtCore, o QtWidgets, o QtQuick, e outros.

Ele possui duas licenças principais: uma LGPL e uma comercial. Os módulos do Qt licenciados como LGPL são de código aberto e permitem que você crie tanto aplicativos de código aberto quanto aplicativos proprietários, de código fechado, gratuitamente, [contanto se siga as condições da licença LGPL](https://www.qt.io/licensing/open-source-lgpl-obligations). Os módulos do Qt licenciados como comerciais fornecem funcionalidade extra e mais facilidades para desenvolvimento e integração em empresas, e o uso desta licença fornece suporte técnico, além de outros serviços. Há alguns poucos módulos que utilizam-se de outras licenças. Por exemplo, módulos que utilizam licença GPL obrigam seu aplicativo a ser de código aberto, embora seja perfeitamente possível lucrar em cima disso, contanto siga-se a licença. Módulos que utilizam licença MIT permitem um uso mais flexível para aplicativos proprietários. Leia [mais sobre isso aqui](https://doc.qt.io/qt-6/licenses-used-in-qt.html). É possível ver quais módulos seguem quais licenças na [página de funcionalidades do Qt](https://www.qt.io/product/features).

</details>

## Qual a diferença entre QtCore, QtWidgets, QtQuick e QML?

<details>
  <summary>Clique aqui para ler</summary>

QtCore é um subconjunto de componentes do Qt especializado em aplicações **sem interface gráfica** (GUI). Ele é usado com C++ (e não QML), mas há language bindings para uso com outras linguagens, como Python. Vários dos seus componentes também estão disponíveis em módulos do QtWidgets e do QtQuick. Sua página inicial da documentação é esta: https://doc.qt.io/qt-6/qtcore-index.html e esta é a sua lista de classes C++: https://doc.qt.io/qt-6/qtcore-module.html. Dentre estas classes, as mais básicas são: [QCoreApplication](https://doc.qt.io/qt-6/qcoreapplication.html), [QDebug](https://doc.qt.io/qt-6/qdebug.html), [QString](https://doc.qt.io/qt-6/qstring.html), [QFile](https://doc.qt.io/qt-6/qfile.html), [QList](https://doc.qt.io/qt-6/qlist.html) e [QVariant](https://doc.qt.io/qt-6/qvariant.html).

QtWidgets é um subconjunto de componentes do Qt especializado em aplicações **com interface gráfica** que oferece integração extra para aplicativos desktop. Ele é usado com C++ (e não QML), mas há language bindings para uso com outras linguagens. Seus componentes principais vem prontos para integrar ao seu sistema opracional. Sua página inicial da documentação é esta: https://doc.qt.io/qt-6/qtwidgets-index.html e esta é a sua lista de classes C++: https://doc.qt.io/qt-6/qtwidgets-module.html. Dentre estas classes, as mais básicas são: [QApplication](https://doc.qt.io/qt-6/qapplication.html), [QWidget](https://doc.qt.io/qt-6/qwidget.html), [QMainWindow](https://doc.qt.io/qt-6/qmainwindow.html), [QDialog](https://doc.qt.io/qt-6/qdialog.html), [QLabel](https://doc.qt.io/qt-6/qlabel.html), [QPushButton](https://doc.qt.io/qt-6/qpushbutton.html), [QRadioButton](https://doc.qt.io/qt-6/qradiobutton.html), [QComboBox](https://doc.qt.io/qt-6/qcombobox.html), [QCheckBox](https://doc.qt.io/qt-6/qcheckbox.html), [QLineEdit](https://doc.qt.io/qt-6/qlineedit.html), [QTextEdit](https://doc.qt.io/qt-6/qtextedit.html), [QLayout](https://doc.qt.io/qt-6/qlayout.html) e [QMenu](https://doc.qt.io/qt-6/qmenu.html).

QtQuick é um subconjunto de componentes do Qt especializado em aplicações **com interface gráfica** que oferece integração extra para aplicativos móveis, além da integração para aplicativos desktop. Ele é usado com QML e opcionalmente C++, mas há language bindings para uso com outras linguagens. Sua página inicial da documentação é esta: https://doc.qt.io/qt-6/qtquick-index.html e esta é a sua lista de classes C++: https://doc.qt.io/qt-6/qtquick-module.html e sua lista de tipos QML: https://doc.qt.io/qt-6/qtquick-qmlmodule.html. As classes C++ possibilitam integrar interfaces QML em programas QtWidgets, enquanto os tipos QML são usados para construir interfaces QML. As duas classes C++ básicas são [QQuickWindow](https://doc.qt.io/qt-6/qquickwindow.html) e [QQuickView](https://doc.qt.io/qt-6/qquickview.html), enquanto seus tipos QML básicos são [Item](https://doc.qt.io/qt-6/qml-qtquick-item.html), [Window](https://doc.qt.io/qt-6/qml-qtquick-window.html), [Rectangle](https://doc.qt.io/qt-6/qml-qtquick-rectangle.html), [Text](https://doc.qt.io/qt-6/qml-qtquick-text.html), [Row](https://doc.qt.io/qt-6/qml-qtquick-row.html), [Column](https://doc.qt.io/qt-6/qml-qtquick-column.html), [Grid](https://doc.qt.io/qt-6/qml-qtquick-grid.html), [Flow](https://doc.qt.io/qt-6/qml-qtquick-flow.html), [ListView](https://doc.qt.io/qt-6/qml-qtquick-listview.html), [Animation](https://doc.qt.io/qt-6/qml-qtquick-animation.html), [Repeater](https://doc.qt.io/qt-6/qml-qtquick-repeater.html) e [Loader](https://doc.qt.io/qt-6/qml-qtquick-loader.html).

QML é uma linguagem declarativa similar ao JSON usada principalmente para criar interfaces gráficas. É possível tanto escrever um programa puramente em QML quanto um programa que misture C++ e QML. Para os que estão familiarizados com a terminologia, a linguagem tem embutido o observer pattern e o composite pattern, e permite utilizar o model-view-controller pattern, state pattern, dentre outros padrões de design de programação, além de implementar um scene graph, o que torna a linguagem versátil e altamente produtiva, isto é, permite produzir mais com menos código.

Existem outros componentes do Qt que interessam para quem pretende programar com o QtQuick: o [QtQuick Layouts](https://doc.qt.io/qt-6/qtquicklayouts-index.html) para criar layouts dinâmicos e o [QtQuick Controls](https://doc.qt.io/qt-6/qtquickcontrols-index.html) para obter controles mais elaborados para sua interface gráfica.

Outros componentes interessantes do Qt são o [QtGUI](https://doc-snapshots.qt.io/qt6-dev/qtgui-overview.html), que fornece alguns componentes de interface essenciais como [QGuiApplication](https://doc-snapshots.qt.io/qt6-dev/qguiapplication.html), [QAction](https://doc-snapshots.qt.io/qt6-dev/qaction.html) e [QColor](https://doc-snapshots.qt.io/qt6-dev/qcolor.html); o [QtQuick3D](https://doc-snapshots.qt.io/qt6-dev/qtquick3d-index.html), que permite trabalhar com modelos 3D usando QML; o [QtWebEngine](https://doc.qt.io/qt-6/qtwebengine-overview.html), que permite trabalhar com páginas da web diretamente, seja com C++ ou QML; e o [Qt for MCUs](https://doc.qt.io/QtForMCUs-2.1/), que foca em aplicativos com interface gráfica em embarcados.

</details>

## Que linguagens posso usar para desenvolver em Qt?

<details>
  <summary>Clique aqui para ler</summary>

A linguagem principal usada para desenvolver em Qt é o C++. O framework em si é feito em C++, assim como a IDE principal do Qt, o QtCreator. Caso queira aprender C++, dê uma olhada no [material de aprendizado do cppbrasil](https://github.com/cppbrasil/material-de-aprendizado).

Também é possível criar programas em Qt usando a linguagem QML. O QML é uma linguagem declarativa similar ao JSON que pode tanto se integrar a código feito em C++ quanto rodar sozinho utilizando expressões JavaScript para a lógica principal. Apesar de utilizar um engine JavaScript em tempo de execução, ele é bastante eficiente e pode ser transpilado para C++ via compilação just-in-time desde o Qt 5.11 (ou [ahead-of-time a partir do Qt 6.3](https://www.qt.io/blog/qml-type-compilation)), fazendo uso da eficiência e velocidade do C++.

A The Qt Company também oficialmente suporta o Python por meio do PySide2 (de Qt5) / PySide6 (de Qt6), [ou Qt For Python](https://wiki.qt.io/Qt_for_Python). Alternativamente, há o [PyQt5 e PyQt6](https://riverbankcomputing.com/software/pyqt/), ambos mantidos pela Riverbank Computers. Este último, no entanto, não recebe suporte da The Qt Company.

Há também [outros language bindings](https://wiki.qt.io/Language_Bindings) para o Qt. Notavelmente, o Rust tem ganhado popularidade recentemente, e para ele estão disponíveis o [Rust-Qt/Ritual](https://rust-qt.github.io/), que fornece bindings Rust -> C++; o [QMetaObject-rs](https://github.com/woboq/qmetaobject-rs), que fornece bindings Rust -> QML; o [Rust-Qt-Binding-Generator](https://invent.kde.org/sdk/rust-qt-binding-generator), desenvolvido pela KDE, que permite criar código feito em Rust que é utilizável em código Qt/QML.
  
Há também o [QtJambi](https://github.com/OmixVisualization/qtjambi/wiki) para Java, o [Qt for Go](https://github.com/therecipe/qt), para Golang, e o [NodeGui](https://github.com/nodegui/nodegui), para NodeJS.

</details>

## Onde/como posso ler a documentação da API do Qt?

<details>
  <summary>Clique aqui para ler</summary>

A documentação do Qt reside em https://doc.qt.io/. É recomendável que você utilize a documentação mais atual, do Qt6, porém a documentação do Qt5 pode ser útil especialmente quando se trata do processo de compilação e gerenciamento de recursos, que foi bastante simplificado com a vinda do Qt6 e a transição do QMake pro CMake.

Há também a [wiki do Qt](https://wiki.qt.io/Main), que pode ser particularmente útil para os recursos mais utilizados. Atente para não acabar visualizando uma página deprecada ou conteúdo que não foi atualizado, que pode comumente ocorrer ao utilizar a pesquisa de um motor de busca como o DuckDuckGo ou o Google.

Caso esteja utilizando o instalador oficial da The Qt Company para instalar o Qt e a sua IDE principal, o QtCreator, você terá toda a documentação disponível no QtCreator offline e por padrão. No lado esquerdo do QtCreator, há uma aba chamada Help que permite acessar toda a documentação. Já no editor, é possível apertar F1 para ativar um painel lateral exibindo a documentação referente ao termo em que o cursor está parado, e apertar F1 novamente irá abrir a página da documentação visualizada, porém na aba Help, usando mais espaço. 

Em sistemas Linux, ao instalar o Qt/QtCreator pelo repositório, a documentação do Qt costuma ser encontrada em /usr/share/docs. Caso não esteja presente após a instalação, geralmente é possível instalar pacotes específicos nos repositórios que contenham os pacotes de documentação, assim como os de exemplos e tutoriais. Os pacotes costumam ter a extensão -doc e a documentação vem como arquivos QCH (formato específico do Qt) ou arquivos HTML. Uma vez presentes no seu sistema, é possível abrir os arquivos diretamente ou ver a documentação no QtCreator.

Caso você utilize o KDevelop, é possível configurar a IDE para que use a documentação instalada em /usr/share/docs de maneira similar ao QtCreator.

Quanto à documentação do Qt em si, você verá que ela é extensa e bastante clara, porém pode ser bastante técnica. Há [três tipos de documentação](https://doc.qt.io/qt-6/explore-qt.html): visão geral, exemplos, e referência de classe C++/tipo QML. Caso esteja começando, veja primeiro as principais páginas de visão geral, que costumam ter explicações detalhadas e exemplos simples, como [Layout Management](https://doc.qt.io/qt-6/layout.html), o [QML Object Attributes](https://doc.qt.io/qt-6/qtqml-syntax-objectattributes.html) ou o [Getting Started with CMake](https://doc.qt.io/qt-6/cmake-get-started.html), por exemplo. Após ler as páginas mais importantes de visão geral da documentação, você pode tentar colocar a mão na massa e replicar os exemplos. Caso esteja difícil, tente ver um canal ou curso introdutório de Qt, ou seguir a Rota de Aprendizado a seguir.

Uma vez que você passar para materiais de referência, como descrições de classes como o [QList](https://doc.qt.io/qt-6/qlist.html) ou tipos como o [ColorAnimation](https://doc.qt.io/qt-5/qml-qtquick-coloranimation.html), lembre-se: para verificar tudo de que uma classe é realmente capaz, clique em "List of all members, including inherited members". Assim é possível ver as propriedades e funções das classes pai, que também podem ser usadas pela classe/tipo sendo visualizada. O ColorAnimation é um bom exemplo disso.

Se você for iniciante e estiver tendo dificuldade com o QtWidgets em particular e sentir como se estivesse faltando alguma informação que parece óbvia mas você não está captando, talvez esteja faltando o conhecimento necessário de C++. Neste caso, você pode acessar o [material de aprendizado do cppbrasil](https://github.com/cppbrasil/material-de-aprendizado) ou focar no QtCore, que é essencialmente um C++ mais agradável de aprender.

</details>

## Rota de aprendizado para iniciantes

<details>
  <summary>Clique aqui para ler</summary>

  Não há muito por aqui ainda. Contribua mandando um pull request! :)
  
  Esta seção irá conter uma referência a conceitos, classes/tipos e links para as referências necessárias em uma sequência razoável para que um iniciante em Qt possa adquirir o conhecimento para criar suas próprias aplicações com alguma independência.
  
  Por enquanto, fique claro: o melhor material para QtQuick/QML atualmente é o [qmlbook](https://www.qt.io/product/qt6/qml-book).
  
  Segue um rascunho dos componentes numa ordem razoável. Falta polir melhor a lista, achar mais overviews e explicar detalhes importantes de cada.
  
  ---
  
### QtCore

#### QCoreApplication

Importância: Alta

Para iniciantes: Aprender como utilizar o construtor e a função exec() é todo o necessário para continuar estudando (isso é válido para o QCoreApplication, QGuiApplication e QApplication). Adicionalmente, aprender as funções usadas para fornecer informações sobre o aplicativo.

Quando retornar: Após aprender sobre signals e slots, verificar as funções quit() e aboutToQuit().

Essencial: Sim

#### qDebug, qInfo, qWarning, qCritical, qFatal

Importância: Alta, Média, Média, Média, Alta

Para iniciantes: Aprender como printar dados na tela. Adicionalmente, aprender os níveis de logging e quando usá-los.

Quando retornar:

Essencial: Sim

#### QString, QChar, QByteArray

Importância: Alta, Média, Alta

Para iniciantes: Focar nas funções de manipulação de strings e de casting.

Quando retornar: Ao estudar QTextStream, assim como quaisquer classes QtWidgets que focam em texto, como QLineEdit e QTextEdit.

Essencial: Sim

#### QStringView, QByteArrayView

Importância: Baixa, Baixa

Para iniciantes: Use sempre que não for modificar uma string.

Quando retornar: Quando estiver confiante em lidar com programas em C++ ou Qt e quiser adicionar uma camada a mais de segurança.

Essencial: Não

#### QTime, QTimeZone, QDate, QDateTime, QCalendar

Importância: Média, Média, Média, Média, Média

Para iniciantes:

Quando retornar: Após aprender sobre timers.

Essencial: Não

#### QRandomGenerator

Importância: Média

Para iniciantes: Focar nas funções generate() e bounded().

Quando retornar:

Essencial: Não

#### QPoint, QLine, QRect, QSize

Importância: Média, Média, Média, Alta

Para iniciantes: O QSize é comumente utilizado como argumento em funções de outras classes do Qt.

Quando retornar: Ao começar a lidar com gráficos e multimídia.

Essencial: Não

#### Object Trees and Ownership - https://doc.qt.io/qt-6/objecttrees.html

Importância: Alta

Para iniciantes: Focar no conceito principal de gerenciamento de memória: se o objeto pai é destruído, seus objetos filhos também são destruídos.

Quando retornar: Sempre que for lidar com QObjects direta ou indiretamente.

Essencial: Sim

#### Signals and Slots - https://doc.qt.io/qt-6/signalsandslots.html

Importância: Alta

Para iniciantes: Focar em: como criar signals e slots, sintaxe do QObject::connect, quando usar this.

Quando retornar: Ao começar a estudar QtWidgets ou QtQuick.

Essencial: Sim

#### QFile, QDir, QUrl, QIODevice, QSettings, QSysInfo, QStandardPaths

Importância: Alta, Alta, Alta, Média, Alta, Baixa, Alta

Para iniciantes: Focar nas funções de abrir e fechar arquivos com QFile, no enum do QIODevice, em como lidar com arquivos ini com QSettings, em como editar arquivos de configuração do usuário via QStandardPaths (por exemplo, arquivos em XDG_CONFIG_DIR no Linux).

Quando retornar: Quando for lidar com documentos como JSON/XML, quando for lidar com QActions, assim como com diálogos do QtWidgets e QtQuick.

Essencial: Sim

#### Qt Namespace - https://doc.qt.io/qt-6/qt.html

Importância: Alta

Para iniciantes: Foque nos enums disponíveis para o Qt e veja as classes pertinentes que os usam.

Quando retornar:

Essencial: Não

#### QFlags - https://doc.qt.io/qt-6/qflags.html

Importância: Baixa

Para iniciantes: Os QFlags são úteis para criar seus próprios enums de maneira segura para uso em classes ou funções.

Quando retornar:

Essencial: Não

#### Container Classes - https://doc.qt.io/qt-6/containers.html

Importância: Alta

Para iniciantes: Se você tiver experiência com classes de container e iteradores da biblioteca padrão, não será difícil acompanhar.

Quando retornar:

Essencial: Sim

#### QList, QVector

Importância: Alta, Baixa

Para iniciantes: Foque no QList do Qt6 e nas suas diferenças com os containers da biblioteca padrão. O QVector foi deprecado pelo QList. Passe um bom tempo se acostumando com o QList.

Quando retornar: Quando for estudar qualquer descendente do QList.

Essencial: Sim

#### QMap, QSet

Importância: Alta, Média

Para iniciantes: Se você tiver experiência com std::map e std::set, não será difícil acompanhar. O QMap será usado extensivamente no futuro, e o QSet fornece algumas funções de conveniência para criar containers facilmente.

Quando retornar: Quando for estudar o QVariant e o QVariantMap, que pode ser usado com QJSon e QXmlStream.

Essencial: Sim

#### QVariant, QIterator

Importância: Alta, Média

Para iniciantes: Se você tiver experiência com std::variant, não será difícil acompanhar. Passe bastante tempo estudando o QVariant, pois ele é necessário para a integração entre código C++ e QML no QtQuick, além de fornecer classes derivadas muito úteis como QVariantList e QVariantMap.

Quando retornar: Ao começar a estudar QtQuick.

Essencial: Sim

#### QStringList, QByteArrayList

Importância: Média, Média

Para iniciantes: Se você tiver praticado lidar com o QList, não será difícil acompanhar. Foque nas diferenças de uso do QString e do QByteArray comparado às suas versões QList, assim como ao QList\<QString\> e QList\<QByteArray\>.

Quando retornar:

Essencial: Não

#### QTextStream

Importância: Baixa

Para iniciantes: Esta classe é particularmente útil para implementar o equivalente a std::cout e std::cin, e age de maneira similar. Se você tiver praticado lidar com QString, QByteArray e QIODevice, não será difícil acompanhar.

Essencial: Não
  
#### QVariantList, QVariantMap

Importância: Alta, Alta

Para iniciantes: Se você tiver praticado lidar com QVariant, não será difícil acompanhar. Passe bastante tempo estudando estas classes, pois elas são usadas bem comumente em programas grandes ou com estruturas de dados complexas, e são necessários para a integração entre código C++ e QML no QtQuick, além de serem úteis com QJSon e QXmlStream.

Quando retornar: Ao começar a estudar QtQuick, ou ao lidar com QJSon e QXmlStream.

Essencial: Sim

#### QCommandLineParser, QCommandLineOption

Importância: Baixa, Média

Para iniciantes: Excetuando o addPositionalArgument() de QCommandLineParser, o construtor e as demais funções são simples. Foque mais no QCommandLineOption e seus construtores. É necessário ter bom entendimento do int argc (contagem de argumentos) e do char* argv[] (vetor/lista de argumentos) e seu papel ao rodar o programa em linha de comando.

Quando retornar:

Essencial: Não

#### QJsonObject, QJsonDocument

Importância: Média, Média

Para iniciantes: Se você tiver praticado lidar com QFile/QIODevice/QStandardPaths, não será difícil acompanhar.

Quando retornar:

Essencial: Não

#### QXmlStreamReader, QXmlStreamWriter

Importância: Média, Média

Para iniciantes: É necessário entendimento do Document Object Model (DOM), além de QFile e QByteArray, e boa prática com iteradores.

Quando retornar:

Essencial: Não

#### QEvent

Importância: Alta

Para iniciantes: De início, basta focar nas opções disponíveis de seu enum. Mais tarde, ao estudar QtWidgets, convém voltar a esta classe para ver suas classes derivadas, uma vez que são necessárias para manipular eventos de interface ou dispositivos de entrada (mouse, teclado).

Quando retornar: Ao lidar com os signals e slots de QtWidgets.

Essencial: Sim

#### Timers, QTimer - https://doc.qt.io/qt-6/timers.html

Importância: Média, Média

Para iniciantes: Excetuando callOnTimeout(), não será difícil acompanhar. Mesmo que para os seus objetivos o QTimer não seja tão útil, a classe permite facilmente testar outras classes conforme são aprendidas.

Quando retornar: Quando você começar a fazer conexões entre eventos mais complexas com QtWidgets.

Essencial: Não

---
  
#### QtWidgets

  ```
QApplication
QWidget, QDialog
QLabel, QLineEdit, QTextEdit, QTextBrowser
QPushButton, QRadioButton, QCheckBox, QComboBox, QSpinBox, QSlider
QDial, QProgressBar
QScrollArea
Layout Management - https://doc.qt.io/qt-6/layout.html
QHBoxLayout, QVBoxLayout, QGridLayout, QFormLayout
QAction
QMainWindow, QMenu, QMenuBar
QToolBar, QTabWidget
QColor, QFont, QIcon, QImage, QStyle
Model/View Programming - https://doc.qt.io/qt-6/model-view-programming.html
Model/View Tutorial - https://doc.qt.io/qt-6/modelview.html
QListView
QColumnView, QTableView, QTreeView
QAbstractItemModel, QModelIndex
QKeyEvent, QShortcut, QValidator
Accessibility for QWidget Applications - https://doc.qt.io/qt-6/accessible-qwidget.html
Internationalization with Qt - https://doc.qt.io/qt-6/internationalization.html  
  ```  
  
</details>


## Canais para seguir

- https://www.youtube.com/c/QtStudios The Qt Company
- https://www.youtube.com/channel/UCpnk1I7ThHtKn4UYkuaO7Qg QtCon Brasil
- https://www.youtube.com/c/KDABtv KDAB TV
- https://www.youtube.com/c/KdeOrg The KDE Community

## Introduções ao Qt

Em Português:
- https://ppgesp.ifba.edu.br/dl47 Introdução ao Qt/QtWidgets (por Sandro Andrade)
- https://agostinhobritojr.github.io/tutorial/qt/index.html Introdução à programação em Qt (por Agostinho Brito Jr.)
- https://www.youtube.com/playlist?list=PLIJWe5QVy1ZpqVmC7DEBoa-8OdxJyg3vY Maratona Qt 2020 (por Sandro Andrade)
- https://youtu.be/QsVqnc6_SgQ QtCon Brasil 2020: Uma Introdução ao Qt for Python (por Mariana Meireles)
- https://www.youtube.com/playlist?list=PL6oOWzm2QNuwGM1gUZkVm79jfvW9QaOpd Playlist introduzindo programação com QtQuick da KDE Brasil (por Patrick Pereira)

Em Inglês:
- https://www.youtube.com/playlist?list=PL6CJYn40gN6hdNC1IGQZfVI707dh9DPRc Introduction to Qt/QML (por KDAB)
- https://youtu.be/Ftm68AzYvr8 Akademy 2021: Qt for Python (por Anupam Basak)

## Cursos completos de Qt

Em Português:
- https://www.youtube.com/playlist?list=PLx4x_zx8csUhzAyii9-cY-IJwo00p_5AC  Curso de Qt (por Canal Fessor Bruno)
- https://www.udemy.com/course/curso-de-qt-moderno-com-cpp-para-linux-e-windows/ Curso de Qt Moderno com C++ (pago, por Marcos Oliveira)

Em Inglês:
- https://www.youtube.com/playlist?list=PL2D1942A4688E9D63 C++ Qt Programming (por Bryan Cairns)
- https://www.youtube.com/playlist?list=PLUbFnGajtZlXbrbdlraCe3LMC_YH5abao Qt 6 With C++ (por Bryan Cairns)

## Livros para aprender Qt

Em Português:
- https://programacaoqt.wordpress.com/ Aprendendo Qt com o projeto Octopi (pago, por Alexandre Albuquerque Arnt)

Em Inglês:
- https://wiki.qt.io/Books Lista extensa de livros ensinando Qt (todos pagos excetuando o qmlbook)
- https://www.qt.io/product/qt6/qml-book O livro de QML6 oficial da TQC baseado no qmlbook de Cadaques
- https://qmlbook.github.io/ O livro de QML5 original por Cadaques

## Tutoriais de Qt oficiais da The Qt Company em Inglês

- https://www.youtube.com/playlist?list=PLizsthdRd0Ywl59atMhNyCydPrb6xz8wN Playlist de tutoriais oficiais da TheQtCompany

O seguinte conteúdo e mais é disponibilizado pela The Qt Company por meio do [Learning Hub](https://resources.qt.io/learning-hub), e é possível encontrar este material no QtCreator.

- https://www.youtube.com/watch?v=-xhiVA0P4yk Qt Windows Online Installer walkthrough
- https://www.youtube.com/watch?v=2RvhhEAZQxM Qt Widgets or Qt Quick
- https://www.youtube.com/watch?v=zAqSiIGdj8M Meet Qt Creator
- https://www.youtube.com/watch?v=R6zWLfHIYJw Introduction to Qt - Qt Creator IDE Overview and Examples {tutorial}
- https://www.youtube.com/watch?v=uuhmSZxK1mk Introduction to Qt – Intro to Qt Quick Controls {tutorial}
- https://www.youtube.com/watch?v=mAhwHsGdJuI Creating a simple QtQuick app (quebrado)
- https://www.youtube.com/watch?v=jbx3Oq1Q4gY Creating a simple widget app
- https://www.youtube.com/watch?v=Y-MM-9FigTc Debugging inside QtCreator
- https://www.youtube.com/watch?v=xNIz78IPBu0 How to do translations with Qt Linguist
- https://www.youtube.com/watch?v=mn-JmXIMCqk How to create a simple application with Qt for MCUs
- https://www.youtube.com/watch?v=BkgjJfxYN20 Build your first 'Qt for MCUs' application
- https://www.youtube.com/watch?v=DRFz0Tll4G8 How to install and set up Qt for MCUs
- https://www.youtube.com/watch?v=YJfFwDBOvqk How to install and set up Qt for Device Creation on Linux
- https://www.youtube.com/watch?v=1tSpq5OLkYI How to set up and deploy an application using Qt for Device Creation
- https://www.youtube.com/watch?v=9BcAYDlpuT8 Using C++ Models in QML {tutorial}
- https://www.youtube.com/watch?v=9xqhq9nDiOg Qt SCXML and state machine tooling in Qt Creator


## Talks de Qt oficiais da The Qt Company em Inglês (material opcional)

<details>
  <summary>Clique aqui para ver o material opcional</summary>

- https://www.youtube.com/watch?v=nmvurCcsWos All You Need to Get Your App Done with Qt for Android | Tools | #QtWS21
- https://www.youtube.com/watch?v=3o2Wo4YzlII QtWS17 - Android & iOS - put your app on a diet, Maciej Węglarczyk, GameDesire
- https://www.youtube.com/watch?v=sRihJdZFuCg Code Once Deploy Everywhere: How Qt is ideal for cross-platform development
- https://www.youtube.com/watch?v=Ko3DuCgFamo QtWS15- Custom Qt Creator Wizards, Tobias Hunger, The Qt Company
- https://www.youtube.com/watch?v=v4glCQt2jE0 QtWS15- Effective multi platform development with Qt, Creator, QBS, and QEMU
- https://www.youtube.com/watch?v=DP0lMoLVneY QtDD13 - Tobias Hunger - Extending Qt Creator
- https://www.youtube.com/watch?v=qclquZ99ZVQ QtWS16- How to Develop with Qt for Multi-Screen and Platforms, Efficient App Lifecycle with Qt
- https://www.youtube.com/watch?v=PzV2MYRAUYQ How to create a plugin for Qt Creator
- https://www.youtube.com/watch?v=v_ynSET9FHU LTTng for full stack tracing
- https://www.youtube.com/watch?v=au3brB7lNms QtWS17 No Limits: HowTo make a more complicated mobile business APP, Ekkehard Gentz
- https://www.youtube.com/watch?v=ECA8_oLT0ZE Qt & Yocto, an ECU development workflow
- https://www.youtube.com/watch?v=TiJiF0MOOFc QtDD14 -Using the QML profiler - Ulf Hermann
- https://www.youtube.com/watch?v=hrKz63Q_Rf0 QtDD13 - Tim Sander - QtCreator for BareMetal development
- https://www.youtube.com/watch?v=1w0ak9RNNWY Qt Creator in Space | Tools | #QtWS21
- https://www.youtube.com/watch?v=B0X5FOev9Lw Qt Designer tutorial: Integrate custom widgets
- https://www.youtube.com/watch?v=X0kEkB0ewyw QtWS16- Qt SCXML: State Machines Made Easier, Ulf Hermann, The Qt Company
- https://www.youtube.com/watch?v=T_13aX5NTPk QtWS16- Qt for iOS A to Z, Mike Krus, KDAB
- https://www.youtube.com/watch?v=tnZo9umrPtg Styling a Qt Quick Controls Desktop Application | User Interface | #QtWS21
- https://www.youtube.com/watch?v=G0AbgVHGdXI QtWS15- The CPU Usage Analyzer for Device Creation, Ulf Herman, The Qt Company
- https://www.youtube.com/watch?v=WIRRoPxIerc QtWS16- The Curse of Choice: An Overview of GUI technologies in Qt, Andy Nichols, The Qt Company
- https://www.youtube.com/watch?v=pN0pRBUqrrc The New Property Bindings: Making C++ more QMLish | Platform | #QtWS21
- https://www.youtube.com/watch?v=W3WC-VpKdGQ WEBASM with Qt - Qt for WebAssembly

</details>
  
## QtCore

Em Português:

Em Inglês:
- https://www.udemy.com/course/qt-6-core-beginners-with-cpp/ Qt6 Core for Beginners with C++ por Bryan Cairns (pago)
- https://www.udemy.com/course/qt-6-core-intermediate/ Qt6 Core Intermediate with C++ por Bryan Cairns (pago)
- https://www.udemy.com/course/qt-6-core-advanced/ Qt6 Core Advanced with C++ por Bryan Cairns (pago)
- https://www.udemy.com/course/qt-core-for-beginners/ Qt5 Core for Beginners with C++ por Bryan Cairns (pago)
- https://www.udemy.com/course/qt-core-intermediate/ Qt5 Core Intermediate with C++ por Bryan Cairns (pago)
- https://www.udemy.com/course/qt-core-advanced/ Qt5 Core Advanced with C++ por Bryan Cairns (pago)

Detalhes adicionais:
- O QtCore serve como excelente porta de entrada para quem sabe bem pouco de C++. Na prática se vê uma API bastante similar à da biblioteca padrão do C++, porém mais legível e fácil de usar.
  
## QtWidgets

Em Português:

Em Inglês:
- https://www.udemy.com/course/qt-widgets-beginners/ Qt5 Widgets for Beginners por Bryan Cairns (pago)
- https://www.udemy.com/course/qt6-c-gui-widgets-tutorial-for-beginners/ Qt6 C++ GUI Development for Beginners por Daniel Gakwaya (pago)
- https://www.udemy.com/course/qt-c-gui-tutorial-for-complete-beginners/ Qt5 C++ GUI Development for Beginners por Daniel Gakwaya (pago)
- https://www.udemy.com/course/qt-c-gui-development-intermediate/ Qt5 C++ GUI Development Intermediate por Daniel Gakwaya (pago)

Detalhes adicionais:
- O QtWidgets vem com widgets praticamente prontos para o desktop. Por padrão integra com o sistema e o tema com quase nenhum esforço.
- Não é apropriado para mobile.
- A nova API do CMake pro Qt6 [qt_standard_project_setup](https://doc.qt.io/qt-6/qt-standard-project-setup.html) tira a necessidade definir manualmente certas configurações do CMake, como AUTOMOC, AUTORCC e AUTOUIC, reduzindo significativamente o tamanho dos arquivos CMake.


## QtQuick

Em Português:
- https://www.youtube.com/playlist?list=PL6oOWzm2QNuwGM1gUZkVm79jfvW9QaOpd Playlist introduzindo programação com QtQuick da KDE Brasil (por Patrick Pereira)
- https://youtu.be/PgmrFTV9ric QtCon Brasil 2020: Prototipagem Rápida com QML (por Patrick Pereira)

Em Inglês:
- https://www.qt.io/product/qt6/qml-book O livro de QML6 oficial da TQC baseado no qmlbook de Cadaques
- https://qmlbook.github.io/ O livro de QML5 original por Cadaques
- https://www.youtube.com/playlist?list=PL6CJYn40gN6hdNC1IGQZfVI707dh9DPRc Introduction to Qt/QML por KDAB
- https://www.youtube.com/playlist?list=PL6CJYn40gN6jWHP5krsQrVGyYtKh3A3be QML Tips and Tricks por KDAB
- https://www.ics.com/events/qml-programming-fundamentals-and-beyond QML Programming Fundamentals and Beyond por ICS
- https://www.udemy.com/course/qml-for-beginners/ QML5 for Beginners por Bryan Cairns (pago)
- https://www.udemy.com/course/qt_quick_qml_tutorial_for_beginners/ Qt Quick and QML for Beginners por Daniel Gakwaya (pago)
- https://www.udemy.com/course/interfacing-qt-quick-qml-to-cpp-intermediate/ Qt Quick and QML Intermediate por Daniel Gakwaya (pago)
- https://www.udemy.com/course/interfacing-qt-quick-qml-to-cpp-advanced/ Qt Quick and QML Advanced por Daniel Gakwaya (pago)
  
Detalhes adicionais:
- O QtQuick vem com widgets mais crus por padrão, requer definir propriedades para integrar ao sistema.
- É a tecnologia recomendada caso for fazer aplicativos mobile.
- A partir do Qt 5.15 e do Qt 6.0 pra frente, é possível [fazer imports sem versionamento](https://doc.qt.io/qt-6/cmake-qt5-and-qt6-compatibility.html#versionless-commands).
- Caso queira verificar as versões das bibliotecas QML que você tem no seu sistema Linux, dentro das pastas /usr/lib64/qt5/qml e /usr/lib64/qt6/qml há arquivos chamados plugins.qmltypes para cada biblioteca. Neles, a versão mínima de cada módulo pode ser vista em linhas contendo a palavra "exports". 
- Lembre-se: filhos de um [Layout](https://doc.qt.io/qt-6/qml-qtquick-layouts-layout.html) devem usar [attached properties](https://doc.qt.io/qt-6/qtqml-syntax-objectattributes.html#attached-properties-and-attached-signal-handlers), não [anchors](https://doc.qt.io/qt-6/qtquick-positioning-anchors.html).
- Lembre-se: nunca use anchors e attached properties ao mesmo tempo no mesmo componente.
- Lembre-se: signals disponíveis ou criados pelo QML automaticamente geram signal handlers do tipo on + Nome (e em certos casos + Changed). Por exemplo, o signal clicked do [QtQuick.Controls Button](https://doc.qt.io/qt-6/qml-qtquick-controls2-button.html) possui o signal handler onClicked; o signal value do [QtQuick.Controls Slider](https://doc.qt.io/qt-6/qml-qtquick-controls2-slider.html) possui o signal handler onValueChanged. Signal handlers NÃO aparecem na documentação de referência do Qt.
- Há certos tipos QML especiais que não precisam de layout ou anchors, como o [Repeater](https://doc.qt.io/qt-6/qml-qtquick-repeater.html), porque internamente eles transferem a relação de pai/filho para cima. Por exemplo, no caso de um [ColumnLayout](https://doc.qt.io/qt-6/qml-qtquick-layouts-columnlayout.html) contendo um Repeater de [Buttons](https://doc.qt.io/qt-6/qml-qtquick-controls2-button.html), os Buttons se tornam filhos diretos do ColumnLayout.
- A nova API do CMake pro Qt6 [qt_add_qml_module](https://doc-snapshots.qt.io/qt6-dev/qt-add-qml-module.html) já cria resources para você, logo não é necessário (nem recomendado) usar o [qt_add_resources](https://doc.qt.io/qt-6/qt-add-resources.html) junto dele.
- Singletons feitos pelo QML usando pragma singleton requerem a propriedade QT_QML_SINGLETON_TYPE definida usandos set_source_files_properties.

## PySide/PyQt

Em Português:
- https://www.youtube.com/playlist?list=PLfQ7GQSrl0_ung_Wt0PpgOICqA8k6dr3i Curso de Python e PySide6 (por Wanderson) 
- https://www.youtube.com/playlist?list=PLtWfwYlJPu5zqNYITJrT9fMyRadOjaxEM Curso de Qt5 PySide2 GUI (por Marcone)
- https://www.youtube.com/playlist?list=PLwsAoT89dh3qJ8JcprQ8AuHY8AGasvx4G Curso de PyQt5 (por Canal Eletrônica e Programação)

Em Inglês:
- https://www.youtube.com/playlist?list=PLfQ7GQSrl0_sD1QIopcYA9GTDUA0nOox5 Qt Quick and Python (por Wanderson)

Detalhes adicionais:
  
## Outros links
Em Português:
- https://github.com/cppbrasil/material-de-aprendizado Materiais de aprendizado para C++
- https://t.me/qtbrasil O grupo oficial do QtBrasil no Telegram

Em Inglês:
- https://github.com/mikeroyal/Qt-Guide Mais recursos ainda para aprender Qt
- https://planet.qt.io/ Agregador global de blogs relacionados ao Qt
- https://qmlonline.kde.org/ Prototipe programas em QML direto pelo navegador
- https://github.com/mikalv/awesome-qt-qml Programas feitos em QtQuick/QML
- https://wiki.manjaro.org/index.php/List_of_Qt_Applications Lista extensa de aplicativos feitos em Qt
- https://inqlude.org/ Lista extensa de bibliotecas feitas em Qt com suporte oficial
- https://insideqt.github.io/awesome-qt/ Mais uma lista extensa de software em Qt
- https://github.com/JesseTG/awesome-qt E mais outra lista extensa de software em Qt
- https://doc.qt.io/qt-6/best-practices.html Coletânea de boas práticas de programação em Qt oficial
- https://github.com/Furkanzmc/QML-Coding-Guide Coletânea de boas práticas de programação em QML
- https://doc.qt.io/archives/qq/qq13-apis.html Explicando o design da API do Qt
- https://wiki.qt.io/API_Design_Principles O material de referência do design da API do Qt


## Contribuindo

<details>
  <summary>Clique aqui para ler</summary>

As diretrizes para contribuir são as seguintes:

* A licença deste readme é GPLv3, porque sim.
* Material em inglês é permitido, **mas dê preferência a material em português brasileiro**, caso exista/você conheça.
* Material pago é permitido, **mas dê preferência a material gratuito**, caso exista. Em toda lista, **o material pago deve aparecer abaixo**.
* Material de Qt4 _de referência_ é permitido apenas como material complementar (ou seja, na seção Outros links ou outra futura para isso).
* Material de Qt4 _que não seja de referência_ é permitido (na seção Outros links ou outra futura para isso).
* Dê prioridade a links, não texto; isso significa que **seções grandes de texto devem ser colapsáveis**. Isso torna todo o material imediatamente acessável sem aumentar o tamanho da página excessivamente.
* Dê preferência a **autores de renome/especialistas**.
* Se o curso for em multimídia, **dê preferência a autores de boa pronúncia/com áudio decente**.
* Materiais complementares de CMake são aceitos, **mas em sua própria seção**.
* Materiais complementares de C++ são aceitos, **mas em sua própria seção**. Prefira contribuir diretamente ao [material de aprendizado do cppbrasil](https://github.com/cppbrasil/material-de-aprendizado) ou ao [livro de C++](https://github.com/tarcisiofischer/livrocpp).
* Caso não haja objeções durante o pull request, o material será incluso. A ideia do repositório é ser completo; **é preferível adicionar antes e vetar depois** do que restringir desnecessariamente a inclusão de material. **A única exceção são cursos pagos**, que precisam de veto para garantir a qualidade antes de serem inclusos.

  </details>
