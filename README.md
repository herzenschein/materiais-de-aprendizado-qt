# Materiais de aprendizado para estudar Qt
Este repositório contém materiais para estudar Qt em português e inglês.

# Qual a diferença entre QtCore, QtWidgets, QtQuick e QML?

QtCore é um subconjunto de componentes do Qt especializado em aplicações **sem interface gráfica** (GUI). Ele é usado com C++ (e não QML), mas há language bindings para uso com outras linguagens, como Python. Vários dos seus componentes também estão disponíveis em módulos do QtWidgets e do QtQuick. Sua página inicial da documentação é esta: https://doc.qt.io/qt-6/qtcore-index.html e esta é a sua lista de classes C++: https://doc.qt.io/qt-6/qtcore-module.html. Dentre estas classes, as mais básicas são: [QCoreApplication](https://doc.qt.io/qt-6/qcoreapplication.html), [QDebug](https://doc.qt.io/qt-6/qdebug.html), [QString](https://doc.qt.io/qt-6/qstring.html), [QFile](https://doc.qt.io/qt-6/qfile.html), [QList](https://doc.qt.io/qt-6/qlist.html) e [QVariant](https://doc.qt.io/qt-6/qvariant.html).

QtWidgets é um subconjunto de componentes do Qt especializado em aplicações **com interface gráfica** que oferece integração extra para aplicativos desktop. Ele é usado com C++ (e não QML), mas há language bindings para uso com outras linguagens. Seus componentes principais vem prontos para integrar ao seu sistema opracional. Sua página inicial da documentação é esta: https://doc.qt.io/qt-6/qtwidgets-index.html e esta é a sua lista de classes C++: https://doc.qt.io/qt-6/qtwidgets-module.html. Dentre estas classes, as mais básicas são: [QApplication](https://doc.qt.io/qt-6/qapplication.html), [QWidget](https://doc.qt.io/qt-6/qwidget.html), [QMainWindow](https://doc.qt.io/qt-6/qmainwindow.html), [QDialog](https://doc.qt.io/qt-6/qdialog.html), [QLabel](https://doc.qt.io/qt-6/qlabel.html), [QPushButton](https://doc.qt.io/qt-6/qpushbutton.html), [QRadioButton](https://doc.qt.io/qt-6/qradiobutton.html), [QComboBox](https://doc.qt.io/qt-6/qcombobox.html), [QCheckBox](https://doc.qt.io/qt-6/qcheckbox.html), [QLineEdit](https://doc.qt.io/qt-6/qlineedit.html), [QTextEdit](https://doc.qt.io/qt-6/qtextedit.html), [QLayout](https://doc.qt.io/qt-6/qlayout.html) e [QMenu](https://doc.qt.io/qt-6/qmenu.html).

QtQuick é um subconjunto de componentes do Qt especializado em aplicações **com interface gráfica** que oferece integração extra para aplicativos móveis, além da integração para aplicativos desktop. Ele é usado com QML e opcionalmente C++, mas há language bindings para uso com outras linguagens. Sua página inicial da documentação é esta: https://doc.qt.io/qt-6/qtquick-index.html e esta é a sua lista de classes C++: https://doc.qt.io/qt-6/qtquick-module.html e sua lista de tipos QML: https://doc.qt.io/qt-6/qtquick-qmlmodule.html. As classes C++ possibilitam integrar interfaces QML em programas QtWidgets, enquanto os tipos QML são usados para construir interfaces QML. As duas classes C++ básicas são [QQuickWindow](https://doc.qt.io/qt-6/qquickwindow.html) e [QQuickView](https://doc.qt.io/qt-6/qquickview.html), enquanto seus tipos QML básicos são [Item](https://doc.qt.io/qt-6/qml-qtquick-item.html), [Window](https://doc.qt.io/qt-6/qml-qtquick-window.html), [Rectangle](https://doc.qt.io/qt-6/qml-qtquick-rectangle.html), [Text](https://doc.qt.io/qt-6/qml-qtquick-text.html), [Row](https://doc.qt.io/qt-6/qml-qtquick-row.html), [Column](https://doc.qt.io/qt-6/qml-qtquick-column.html), [Grid](https://doc.qt.io/qt-6/qml-qtquick-grid.html), [Flow](https://doc.qt.io/qt-6/qml-qtquick-flow.html), [ListView](https://doc.qt.io/qt-6/qml-qtquick-listview.html), [Animation](https://doc.qt.io/qt-6/qml-qtquick-animation.html), [Repeater](https://doc.qt.io/qt-6/qml-qtquick-repeater.html) e [Loader](https://doc.qt.io/qt-6/qml-qtquick-loader.html).

# Que linguagens posso usar para desenvolver em Qt?

...

<!-- Não esquecer de mencionar o material do C++ Brasil aqui -->

# Onde/como posso ler a documentação da API do Qt?

...

# Rota de aprendizado para iniciantes

...

<!-- 
Adicionar uma sugestão de rota de aprendizado de componentes de QtCore/QtWidgets/QtQuick para iniciantes.
-->

# Canais para seguir
- https://www.youtube.com/c/QtStudios The Qt Company
- https://www.youtube.com/channel/UCpnk1I7ThHtKn4UYkuaO7Qg QtCon Brasil
- https://www.youtube.com/c/KDABtv KDAB TV
- https://www.youtube.com/c/KdeOrg The KDE Community

# Introduções ao Qt
Em Português:
- https://ppgesp.ifba.edu.br/dl47 Introdução ao Qt/QtWidgets (por Sandro Andrade)
- https://agostinhobritojr.github.io/tutorial/qt/index.html Introdução à programação em Qt (por Agostinho Brito Jr.)
- https://programacaoqt.wordpress.com/ Aprendendo Qt com o projeto Octopi (por Alexandre Albuquerque Arnt)
- https://www.youtube.com/playlist?list=PLIJWe5QVy1ZpqVmC7DEBoa-8OdxJyg3vY Maratona Qt 2020 (por Sandro Andrade)
- https://www.youtube.com/playlist?list=PLx4x_zx8csUhzAyii9-cY-IJwo00p_5AC  Curso de Qt (por Canal Fessor Bruno)
- https://www.youtube.com/playlist?list=PLtWfwYlJPu5zqNYITJrT9fMyRadOjaxEM Curso de Qt5 PySide2 GUI (por Marcone)

Em Inglês:

- https://www.youtube.com/playlist?list=PL6CJYn40gN6hdNC1IGQZfVI707dh9DPRc Introduction to Qt/QML (por KDAB)
- https://www.youtube.com/playlist?list=PL2D1942A4688E9D63 C++ Qt Programming (por Bryan Cairns)
- https://www.youtube.com/playlist?list=PLUbFnGajtZlXbrbdlraCe3LMC_YH5abao Qt 6 With C++ (por Bryan Cairns)

# Tutoriais de Qt oficiais da The Qt Company em Inglês

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


# Talks de Qt oficiais da The Qt Company em Inglês

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

# QtCore
Em Português:

Em Inglês:


# QtWidgets
Em Português:

Em Inglês:


# QtQuick
Em Português:

Em Inglês:


# Outros links
Em Português:
- https://github.com/cppbrasil/material-de-aprendizado Materiais de aprendizado para C++

Em Inglês:
- https://github.com/mikalv/awesome-qt-qml Programas feitos em QtQuick/QML
