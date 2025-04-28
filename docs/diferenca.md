# Qual a diferença entre QtCore, QtWidgets, QtQuick e QML?

## Sobre o QtCore

QtCore é um subconjunto de componentes do Qt especializado em aplicações **sem interface gráfica** (GUI). Ele é usado com C++ (e não QML), mas há language bindings para uso com outras linguagens, como Python. Vários dos seus componentes também estão disponíveis em módulos do QtWidgets e do QtQuick.

A página inicial da documentação do QtCore é esta: [https://doc.qt.io/qt-6/qtcore-index.html](https://doc.qt.io/qt-6/qtcore-index.html)

A lista de classes C++ do QtCore é esta: [https://doc.qt.io/qt-6/qtcore-module.html](https://doc.qt.io/qt-6/qtcore-module.html).

Dentre estas classes, as mais básicas são:

* [QCoreApplication](https://doc.qt.io/qt-6/qcoreapplication.html)
* [QDebug](https://doc.qt.io/qt-6/qdebug.html)
* [QString](https://doc.qt.io/qt-6/qstring.html)
* [QFile](https://doc.qt.io/qt-6/qfile.html)
* [QList](https://doc.qt.io/qt-6/qlist.html)
* [QVariant](https://doc.qt.io/qt-6/qvariant.html)

---

## Sobre o QtWidgets

QtWidgets é um subconjunto de componentes do Qt especializado em aplicações **com interface gráfica** que oferece integração extra para aplicativos desktop. Ele é usado com C++ (e não QML), mas há language bindings para uso com outras linguagens. Seus componentes principais vem prontos para integrar ao seu sistema opracional.

A página inicial da documentação do QtWidgets: [https://doc.qt.io/qt-6/qtwidgets-index.html](https://doc.qt.io/qt-6/qtwidgets-index.html)

A lista de classes C++ do QtWidgets: [https://doc.qt.io/qt-6/qtwidgets-module.html](https://doc.qt.io/qt-6/qtwidgets-module.html)

Dentre estas classes, as mais básicas são:

* [QApplication](https://doc.qt.io/qt-6/qapplication.html)
* [QWidget](https://doc.qt.io/qt-6/qwidget.html)
* [QMainWindow](https://doc.qt.io/qt-6/qmainwindow.html)
* [QDialog](https://doc.qt.io/qt-6/qdialog.html)
* [QLabel](https://doc.qt.io/qt-6/qlabel.html)
* [QPushButton](https://doc.qt.io/qt-6/qpushbutton.html)
* [QRadioButton](https://doc.qt.io/qt-6/qradiobutton.html)
* [QComboBox](https://doc.qt.io/qt-6/qcombobox.html)
* [QCheckBox](https://doc.qt.io/qt-6/qcheckbox.html)
* [QLineEdit](https://doc.qt.io/qt-6/qlineedit.html)
* [QTextEdit](https://doc.qt.io/qt-6/qtextedit.html)
* [QLayout](https://doc.qt.io/qt-6/qlayout.html)
* [QMenu](https://doc.qt.io/qt-6/qmenu.html).

---

## Sobre o QtQuick

QtQuick é um subconjunto de componentes do Qt especializado em aplicações **com interface gráfica** que oferece integração extra para aplicativos móveis, além da integração para aplicativos desktop. Ele é usado com QML e opcionalmente C++, mas há language bindings para uso com outras linguagens.

A página inicial da documentação do QtQuick: https://doc.qt.io/qt-6/qtquick-index.html

A lista de classes C++ do QtQuick: https://doc.qt.io/qt-6/qtquick-module.html

A lista de tipos QML do QtQuick: https://doc.qt.io/qt-6/qtquick-qmlmodule.html

As classes C++ possibilitam integrar interfaces QML em programas QtWidgets, enquanto os tipos QML são usados para construir interfaces QML.

As duas classes C++ básicas são:

* [QQuickWindow](https://doc.qt.io/qt-6/qquickwindow.html)
* [QQuickView](https://doc.qt.io/qt-6/qquickview.html)

Enquanto seus tipos QML básicos são:

* [Item](https://doc.qt.io/qt-6/qml-qtquick-item.html)
* [Window](https://doc.qt.io/qt-6/qml-qtquick-window.html)
* [Rectangle](https://doc.qt.io/qt-6/qml-qtquick-rectangle.html)
* [Text](https://doc.qt.io/qt-6/qml-qtquick-text.html)
* [Row](https://doc.qt.io/qt-6/qml-qtquick-row.html)
* [Column](https://doc.qt.io/qt-6/qml-qtquick-column.html)
* [Grid](https://doc.qt.io/qt-6/qml-qtquick-grid.html)
* [Flow](https://doc.qt.io/qt-6/qml-qtquick-flow.html)
* [ListView](https://doc.qt.io/qt-6/qml-qtquick-listview.html)
* [Animation](https://doc.qt.io/qt-6/qml-qtquick-animation.html)
* [Repeater](https://doc.qt.io/qt-6/qml-qtquick-repeater.html)
* [Loader](https://doc.qt.io/qt-6/qml-qtquick-loader.html)

---

## Sobre o QML

QML é uma linguagem declarativa similar ao JSON usada principalmente para criar interfaces gráficas. É possível tanto escrever um programa puramente em QML quanto um programa que misture C++ e QML. Para os que estão familiarizados com a terminologia, a linguagem tem embutido o observer pattern e o composite pattern, e permite utilizar o model-view-controller pattern, state pattern, dentre outros padrões de design de programação, além de implementar um scene graph, o que torna a linguagem versátil e altamente produtiva, isto é, permite produzir mais com menos código.

---

Existem outros componentes do Qt que interessam para quem pretende programar com o QtQuick: o [QtQuick Layouts](https://doc.qt.io/qt-6/qtquicklayouts-index.html) para criar layouts dinâmicos e o [QtQuick Controls](https://doc.qt.io/qt-6/qtquickcontrols-index.html) para obter controles mais elaborados para sua interface gráfica.

Outros componentes interessantes do Qt são o [QtGUI](https://doc-snapshots.qt.io/qt6-dev/qtgui-overview.html), que fornece alguns componentes de interface essenciais como [QGuiApplication](https://doc-snapshots.qt.io/qt6-dev/qguiapplication.html), [QAction](https://doc-snapshots.qt.io/qt6-dev/qaction.html) e [QColor](https://doc-snapshots.qt.io/qt6-dev/qcolor.html); o [QtQuick3D](https://doc-snapshots.qt.io/qt6-dev/qtquick3d-index.html), que permite trabalhar com modelos 3D usando QML; o [QtWebEngine](https://doc.qt.io/qt-6/qtwebengine-overview.html), que permite trabalhar com páginas da web diretamente, seja com C++ ou QML; e o [Qt for MCUs](https://doc.qt.io/QtForMCUs-2.1/), que foca em aplicativos com interface gráfica em embarcados.
