# Que linguagens posso usar para desenvolver em Qt?

A linguagem principal usada para desenvolver em Qt é o C++. O framework em si é feito em C++, assim como a IDE principal do Qt, o QtCreator. Caso queira aprender C++, dê uma olhada no [material de aprendizado do cppbrasil](https://github.com/cppbrasil/material-de-aprendizado).

Também é possível criar programas em Qt usando a linguagem QML. O QML é uma linguagem declarativa similar ao JSON que pode tanto se integrar a código feito em C++ quanto rodar sozinho utilizando expressões JavaScript para a lógica principal. Apesar de utilizar um engine JavaScript em tempo de execução, ele é bastante eficiente e pode ser transpilado para C++ via compilação just-in-time desde o Qt 5.11 (ou [ahead-of-time a partir do Qt 6.3](https://www.qt.io/blog/qml-type-compilation)), fazendo uso da eficiência e velocidade do C++.

A The Qt Company também oficialmente suporta o Python por meio do PySide2 (de Qt5) / PySide6 (de Qt6), [ou Qt For Python](https://wiki.qt.io/Qt_for_Python). Alternativamente, há o [PyQt5 e PyQt6](https://riverbankcomputing.com/software/pyqt/), ambos mantidos pela Riverbank Computers. Este último, no entanto, não recebe suporte da The Qt Company.

Há também [outros language bindings](https://wiki.qt.io/Language_Bindings) para o Qt. Notavelmente, o Rust tem ganhado popularidade recentemente, e para ele estão disponíveis o [Rust-Qt/Ritual](https://rust-qt.github.io/), que fornece bindings Rust -> C++; o [QMetaObject-rs](https://github.com/woboq/qmetaobject-rs), que fornece bindings Rust -> QML; o [Rust-Qt-Binding-Generator](https://invent.kde.org/sdk/rust-qt-binding-generator), desenvolvido pela KDE, que permite criar código feito em Rust que é utilizável em código Qt/QML.
  
Há também o [QtJambi](https://github.com/OmixVisualization/qtjambi/wiki) para Java, o [Qt for Go](https://github.com/therecipe/qt), para Golang, e o [NodeGui](https://github.com/nodegui/nodegui), para NodeJS.
